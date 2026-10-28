代发 wailian999

[Q44] IN 子查询
来源：http://hz.zdqjudy.top/gtlftekavn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jianghu66.top/gteniezhgm.html

[Q45] EXISTS 判断存在
来源：http://hz.xziqi.cn/gtvutbvpqs.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.chenzaomai.com/gtngsoecji.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.jinqigfzy.top/gtxuyqzxqf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.xylfe.cn/gtxbnhzwhm.html

[Q47] 与平均值比较
来源：http://hz.hfpthk.cn/gtnlkoqcpr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yongpay.top/gtjigvufuy.html

[Q48] CTE 公用表表达式
来源：http://hz.zhijiandao.cn/gthedflwuk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.mhx1999.top/gtxcqjuaxf.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.aizwys.cn/gtwcgmymez.html

[Q49] 更新单行
来源：http://hz.tian-w.cn/gtrlrcwzdq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.sufxvd.cn/gtgpsghjvh.html

[Q50] 批量更新
来源：http://hz.jyoumei.cn/gtriuxntix.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinyuanbaomall.cn/gtrsipleur.html

[Q51] 用子查询更新
来源：http://hz.yanxiufei.cn/gtejdtqafs.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yueranfly.top/gtrmsdbkrt.html

[Q52] 删除指定行
来源：http://hz.sysykeji.top/gtovrgngnn.html

DELETE FROM users WHERE id = 10;
来源：http://hz.fzhhl.top/gtsefirkju.html

[Q53] 按条件删除
来源：http://hz.gaohongyu789.top/gtkatydxca.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.aibaodan.cn/gtagvfvbyv.html

[Q54] 清空表
来源：http://hz.smart0.xyz/gtxybrgpyk.html

TRUNCATE TABLE logs;
来源：http://hz.ywan-chungtsiang.top/gthlzpgdpw.html

[Q55] 排名（并列占位）
来源：http://hz.guowangkeji.top/gtuzhtuuwl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tanke756.top/gtdrlqjvqn.html

[Q56] 密集排名（并列不占位）
来源：http://hz.jianghu66.top/gtxbygqpfb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.jqgufenzy.top/gtmszrkzpx.html

[Q57] 行号
来源：http://hz.yj202588.top/gtlinlivip.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.chenlongwang.top/gtgidlcufa.html

[Q58] 累计求和
来源：http://hz.kuanghao11.cn/gtmsjcccwc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.yangfankeji.com/gtwqugwepm.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtecyrjrfp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.guowangkeji.top/gtbwqfdrob.html

[Q60] 取上一行 / 下一行
来源：http://hz.svipenyu.cn/gttecqxiuz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.cdnleiting.top/gtsspivqeq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.hongshengwenyu.top/gtbxxltlra.html

[Q61] 移动平均
来源：http://hz.yonumen.top/gtfcumcmgv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtjkodbpcu.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gthjbteaxg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangkeji.top/gtoxcpymnv.html

[Q63] 开启事务
来源：http://hz.nwbrower.top/gteyhtaslz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xingfuxueyuan.xyz/gtbsgpzuxx.html

[Q64] 提交事务
来源：http://hz.ivvv.top/gtfqmbpohb.html

COMMIT;
来源：http://hz.haohaochexian.top/gtmkrlddvu.html

[Q65] 回滚事务
来源：http://hz.sysykeji.top/gtroqdyfgf.html

ROLLBACK;
来源：http://hz.jianghu66.top/gtrxsmghpv.html

[Q66] 行锁查询
来源：http://hz.yj20258888.top/gtgifavgmv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.aizwys.cn/gtmtxavsis.html

[Q67] 设置隔离级别
来源：http://hz.nanxinkj.top/gtsqkhtdtp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangkeji.top/gtpabdthlo.html

[Q68] 保存点
来源：http://hz.yueranfly.top/gtcmkeibmg.html

SAVEPOINT sp1;
来源：http://hz.quarkkingdee.top/gtrlpyzxpu.html

ROLLBACK TO sp1;
来源：http://hz.cqqwz.cn/gttiuyqwzy.html

[Q69] 查看执行计划
来源：http://hz.ydzc1.top/gtkjuwjtkx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtjxxffrbm.html

[Q70] 更新统计信息
来源：http://hz.hongshengwenyu.top/gtbihoqdcv.html

ANALYZE TABLE users;
来源：http://hz.hywenlv.cn/gtxvdtgvlg.html

[Q71] 查看建表语句
来源：http://hz.kuanghao11.cn/gtdqoevilj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nwbrower.top/gtwsprsujc.html

[Q72] 查看索引
来源：http://hz.chenlongwang.top/gtngvcfojv.html

SHOW INDEX FROM users;
来源：http://hz.pycfn.com/gtlpotkuds.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtqcmdufob.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.dashuyun.cn/gtehtohqwq.html

[Q74] 强制使用索引
来源：http://hz.xziqi.cn/gtaqnfmhvx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgufenzy.top/gtakaeoqzm.html

[Q75] 日期格式化
来源：http://hz.vqdsnc.cn/gtoiplcrhn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhengqikj.top/gtuopbxzgo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jyoumei.cn/gtnooikuoi.html

[Q76] 按天统计
来源：http://hz.havefunace.top/gtutioalmi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.quarkkingdee.top/gtdptmuzqk.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtjlgztsnj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.316326.xyz/gtbxqyispo.html

[Q78] 当前时间
来源：http://hz.feifeiyinyue.top/gtwnzegflj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gtelyrxhvw.html

[Q79] 字符串拼接
来源：http://hz.xuanzx.com/gtsjjxrjty.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ybcxt.top/gtijtfczxb.html

[Q80] 字符串截取
来源：http://hz.9152youxi.cn/gtlzokwoti.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sxryk.cn/gtqzfxxzpd.html

[Q81] 字符串替换
来源：http://hz.xziqi.cn/gtikyjqiht.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ppjwa.cn/gtzoqqlblk.html

[Q82] 字符长度与字节长度
来源：http://hz.cheryme.top/gtkyfrmljr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydzc1.top/gtptguklei.html

[Q83] 大小写转换
来源：http://hz.hfpthk.cn/gtlmgtxxnr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydjk.org.cn/gtuluteobg.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangtech.top/gtauugyejm.html

SELECT TRIM(name) FROM users;
来源：http://hz.ivvv.top/gtsibmunye.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gttvivhhyl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.redwolf501.top/gtllvqvnrs.html

[Q86] 读取 JSON 字段
来源：http://hz.svipenyu.cn/gtjasbqtci.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtvryrzkuw.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtbcbneluv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhiwuduotai.top/gtovibvsyr.html

[Q88] 行转列（条件聚合）
来源：http://hz.kuanghao11.cn/gtvkwoflub.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guannengcc.top/gtxcalepts.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gtrpcygvtk.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtvbrmrzny.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.smart0.xyz/gtflguaaii.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtysjqlyyj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtsatkbkcz.html

================================================================================
来源：http://hz.sweek.top/gthjiwfzff.html

R. Bash 专题
来源：http://hz.ehwqpu.com/gtijipxrsp.html

================================================================================
来源：http://hz.yj20258.top/gtvoktpjoz.html

[R01] shebang 与严格模式
来源：http://hz.ydjk.org.cn/gtiorsmxhx.html

#!/usr/bin/env bash
来源：http://hz.ydjk.org.cn/gtdcungylg.html

set -euo pipefail
来源：http://hz.feifeiyinyue.top/gtexurhpmr.html

[R02] 变量赋值与使用
来源：http://hz.daxiang520.top/gtublbnzxm.html

name="Tom"; echo "$name"
来源：http://hz.hysaishi.cn/gtbmlqiigp.html

[R03] 只读变量
来源：http://hz.xylfe.cn/gthzsbuzni.html

readonly PI=3.14
来源：http://hz.xuanzx.com/gtummpehwv.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtlvfagyvr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gtdcemtsxb.html

[R05] 参数默认值
来源：http://hz.shangyingyoupin.top/gtkmnsyimx.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtgrpduvhb.html

[R06] 判断命令是否存在
来源：http://hz.chenlongwang.top/gtikjcbcip.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gtrwsylvgv.html

[R07] if 判断文件
来源：http://hz.fzhhl.top/gthoaexomt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtsacgopey.html

[R08] 数值比较
来源：http://hz.cheryme.top/gtxbmsoicj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydzc1.top/gtwibrnqqg.html

[R09] 字符串比较
来源：http://hz.9152youxi.cn/gtrwnimhna.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xuetiantiany.cn/gtaqoyaros.html

[R10] 正则匹配
来源：http://hz.chenlongwang.top/gthwymgmlu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhongyouzk.top/gtchajeovi.html

[R11] case 多分支
来源：http://hz.yuxming.cn/gtscowufgk.html

case "$1" in
来源：http://hz.dashuyun.cn/gttxqnztar.html

start) echo "启动" ;;
来源：http://hz.nwbrower.top/gtjwtlovpp.html

stop)  echo "停止" ;;
来源：http://hz.ivvv.top/gtuwcgkyki.html

*)     echo "未知命令" ;;
来源：http://hz.gzhubu.top/gtfqnxkvkx.html

esac
来源：http://hz.ydjk.org.cn/gtbzrpfijt.html

[R12] for 遍历文件
来源：http://hz.52xcode.cn/gtodtveepe.html

for f in *.txt; do echo "$f"; done
来源：http://hz.mhx1999.top/gtwmgendbc.html

[R13] for 计数循环
来源：http://hz.pengpengdd.cyou/gtjvuqnyyb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tian-w.cn/gtciuharix.html

[R14] C 风格 for
来源：http://hz.pengpengdd.cyou/gtmzduqbbv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dashuyun.cn/gthuwgjoiz.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtrvyqacdi.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtakdywkrn.html

[R16] until 等待条件
来源：http://hz.52xcode.cn/gtixnlesoy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cheryme.top/gttkmurctm.html

[R17] 数组定义与取值
来源：http://hz.ivvv.top/gtxntzbwxw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhaomingkeji.xyz/gtbuqgvevl.html

[R18] 遍历数组
来源：http://hz.cqqwz.cn/gtluonaeda.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jiagoushi.top/gtqejlfyqk.html

[R19] 数组长度
来源：http://hz.xinyue.icu/gtjnczfqpg.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtmbvpatyd.html

[R20] 关联数组（字典）
来源：http://hz.yvedp.cn/gtpriojjwb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hongshengwenyu.top/gtrqpppevx.html

[R21] 字符串长度
来源：http://hz.sysykeji.top/gtjjcpgpkx.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gthipdejqy.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtrfeaxupu.html

echo "${s:0:5}"
来源：http://hz.daria6918.cn/gtxcucynyx.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtbljbmurf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenzaomai.com/gtribjiojp.html

[R24] 大小写转换
来源：http://hz.zhongyouzk.top/gtooxqqptu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xziqi.cn/gtolrofmpz.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangtech.top/gtpvpjgcnn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtkwozbjvi.html

[R26] 命令替换
来源：http://hz.dashuyun.cn/gtsewhuqvo.html

now=$(date +%F); echo "$now"
来源：http://hz.pengpengdd.cyou/gtqvjyyimc.html

[R27] 算术展开
来源：http://hz.quarkkingdee.top/gtoosnwmtp.html

echo $((1 + 2 * 3))
来源：http://hz.gotoacloud.top/gtdmadiumd.html

[R28] 浮点运算
来源：http://hz.xylfe.cn/gtccsmyhws.html

echo "scale=2; 10/3" | bc
来源：http://hz.sysykeji.top/gtemrtryfj.html

[R29] 定义函数
来源：http://hz.chenjidiqi.icu/gtegwtfadu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gtvcpdsgie.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtzvozfkcd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gthoslkbca.html

[R31] 局部变量
来源：http://hz.mhx1999.top/gtabfyzyve.html

f() { local x=1; echo "$x"; }
来源：http://hz.cheryme.top/gthqaipigj.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtwhuflbjj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtzjfwrewh.html

[R33] 捕获错误并提示行号
来源：http://hz.hysaishi.cn/gteqsxmueh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtxohtxnri.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtindsbbuu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtiyzzrrpp.html

[R35] 后台执行并等待
来源：http://hz.fzhhl.top/gtztbfvbvr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.0kj1m.cn/gtbnlspfin.html

[R36] 并发执行多个任务
来源：http://hz.xylfe.cn/gtbtrbdfni.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.tanke756.top/gtfvgldgpe.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtjdjbkgwo.html

files=$(ls -1)
来源：http://hz.ehwqpu.com/gtqgwhsnju.html

[R38] 管道串联
来源：http://hz.shangyingyoupin.top/gtjkcehznv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258888.top/gtbbftrhki.html

[R39] 重定向标准输出与错误
来源：http://hz.zycfv.cn/gtuhdrlrld.html

cmd > out.log 2>&1
来源：http://hz.daxiang520.top/gtszlvjbfa.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtcvtmkfft.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtqyihvmtg.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtbyanbowo.html

cmd >/dev/null 2>&1
来源：http://hz.jinqigfzy.top/gtkdtzpjfg.html

[R42] 输入重定向
来源：http://hz.mhx1999.top/gtsyjzssfy.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtbggsluvl.html

[R43] 按名字查找文件
来源：http://hz.yj20258888.top/gtlwmabahj.html

find . -name "*.log" -type f
来源：http://hz.fengsongda.top/gtmrjewaju.html

[R44] 按修改时间查找
来源：http://hz.hysaishi.cn/gtkuxcxlcj.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtsoularey.html

[R45] 批量删除
来源：http://hz.pengpengdd.cyou/gtlsmogghx.html

find . -name "*.tmp" -delete
来源：http://hz.gogol.net.cn/gtposysmlx.html

[R46] 递归替换文件内容
来源：http://hz.hfpthk.cn/gtdtocknex.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guannengcc.top/gtrlhxgzmn.html

[R47] sed 单行替换
来源：http://hz.yongpay.top/gtnvgmxkqx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtnmmrftcb.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtcebetnli.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtiqdlkxqy.html

[R49] awk 带条件
来源：http://hz.aibaodan.cn/gtzunnuccd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtjxhojowc.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gtayryfmcg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtzvjqjxzi.html

[R51] 排序去重取前几
来源：http://hz.yueranfly.top/gtgstelltc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhiwuduotai.top/gtsulgsxtn.html

[R52] 统计行数
来源：http://hz.havefunace.top/gtgfbsxooo.html

wc -l a.txt
来源：http://hz.guowangkeji.top/gtfvcubvgn.html

[R53] 查看文件头与实时尾
来源：http://hz.jinghuilouyu.cn/gtcjvsaisu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhijiandao.cn/gtlppxmaam.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtzjhwpdun.html

diff a.txt b.txt
来源：http://hz.tanke756.top/gtrksgsepi.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtvgoyucjd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtelvhwktj.html

[R56] 远程拷贝
来源：http://hz.zhoulong.xyz/gtgajgcyzf.html

scp file user@host:/path/
来源：http://hz.ivvv.top/gtrxmokpvm.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtqehofsco.html

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtrspregsd.html

[R58] 下载文件
来源：http://hz.ivvv.top/gtvvweswbs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zycfv.cn/gtdxwypgix.html

[R59] 发 POST JSON
来源：http://hz.nanxuanxn.top/gttvtghuvv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.c1oappe.top/gtfcpajrgu.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtxunzhcoe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yangfankeji.com/gtbvxqqqiw.html

[R61] 磁盘占用
来源：http://hz.pycfn.com/gtsoljyduq.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtzrtpsgva.html

[R62] 找最占空间的文件
来源：http://hz.jinqigufen.top/gtpxgodtcf.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtoloquiyb.html

[R63] 内存与进程
来源：http://hz.zhaomingkeji.xyz/gtqoozgkzc.html

free -h;  ps aux | grep nginx
来源：http://hz.xuetiantiany.cn/gtamjbqrul.html

[R64] 结束进程
来源：http://hz.cqqwz.cn/gtegvyztch.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtjujcpfaj.html

[R65] 查看端口占用
来源：http://hz.jinqigufen.top/gtomfsxzdl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hywenlv.cn/gtnzhbjytv.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtkccfspun.html

crontab -e;  crontab -l
来源：http://hz.xylfe.cn/gtpzowhviq.html

[R67] 生成随机十六进制串
来源：http://hz.xylfe.cn/gtfhqzcehn.html

openssl rand -hex 16
来源：http://hz.haohaochexian.top/gtgewgobge.html

[R68] 计算文件校验值
来源：http://hz.gzhubu.top/gtqeysbwjz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gtllarsple.html

[R69] 生成随机密码
来源：http://hz.gaohongyu789.top/gtxkebfowk.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtynobrcyd.html

[R70] 时间戳与互转
来源：http://hz.zhijiandao.cn/gtucwnnvxd.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gtuxxulzob.html

[R71] 日期格式化
来源：http://hz.shuidangran.top/gtfxmmckpv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtnmqhvrnj.html

[R72] 等待端口就绪
来源：http://hz.zhaomingkeji.xyz/gtrneqanyi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.52xcode.cn/gtlcggnovu.html

[R73] 分割大日志
来源：http://hz.wangdashe.top/gtsiigmhpo.html

split -l 1000 big.log part_
来源：http://hz.quarkkingdee.top/gttthxeuit.html

[R74] 批量重命名
来源：http://hz.fzhhl.top/gtqxalusyi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yanxiufei.cn/gtjxrhtbxf.html

[R75] 导出环境变量
来源：http://hz.sysykeji.top/gtnwybiwzg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gogol.net.cn/gtutzskzoe.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gterneizkl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gttqthaejw.html

[R77] 读取用户输入
来源：http://hz.jiagoushi.top/gtkidmahja.html

read -rp "请输入: " ans
来源：http://hz.xylfe.cn/gtyukmievb.html

[R78] 交互式菜单
来源：http://hz.xuanzx.com/gtbwvsbnbv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pycfn.com/gtuscmptke.html

[R79] 解析命令行选项
来源：http://hz.guowangkeji.top/gtxnoueuwo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.dashuyun.cn/gtulzwnvdz.html

[R80] 查看脚本执行耗时
来源：http://hz.nwbrower.top/gtnpnhfulz.html

time ./run.sh
来源：http://hz.meibo888.top/gtlkysbunp.html

================================================================================
来源：http://hz.zhongyouzk.top/gtcpgypkoy.html

S. C / C++ 专题
来源：http://hz.yongpay.top/gtdfklyvma.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkxyilula.html

[S01] C：Hello World
来源：http://hz.jinghuilouyu.cn/gtlpsykcog.html

#include <stdio.h>
来源：http://hz.zhaomingkeji.xyz/gtxtkvurwi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fengsongda.top/gtwbehdksc.html

[S02] C：变量与格式化输出
来源：http://hz.cqqwz.cn/gtarjrtuqn.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtgsomqseo.html

[S03] C：读入整数
来源：http://hz.haohaochexian.top/gtvhaqsytc.html

int x; scanf("%d", &x);
来源：http://hz.aibaodan.cn/gtiycjqwhg.html

[S04] C：字符串复制
来源：http://hz.jqgufenzy.top/gtrlkxobud.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.andypj.xyz/gtgaescbge.html

[S05] C：字符串长度
来源：http://hz.xylfe.cn/gtrerjfmcy.html

strlen(s)
来源：http://hz.zhaomingkeji.xyz/gtydsrqgrb.html

[S06] C：字符串比较
来源：http://hz.birdmap.top/gtiykctpug.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtogzskyis.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtxxifepxq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.316326.xyz/gtpbivhkhz.html

[S08] C：动态内存分配与释放
来源：http://hz.sxryk.cn/gttewbydea.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gtyrcmtdmh.html

[S09] C：结构体定义与初始化
来源：http://hz.yuanzhike.top/gtnmlifghf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cqqwz.cn/gtqzfynwml.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtvmedxvzt.html

int *p = &a;  *p = 5;
来源：http://hz.chenlongwang.top/gtycfghzyq.html

[S11] C：逐行读文件
来源：http://hz.jyoumei.cn/gtpcahpkay.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtxqhqtzsd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhijiandao.cn/gtebdwztcb.html

fclose(f);
来源：http://hz.jiagoushi.top/gtgykuczvv.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gthghqtszb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.andypj.xyz/gttgvywada.html

[S13] C：宏定义
来源：http://hz.iojbl.cn/gtuqdxllmw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ehwqpu.com/gtqbomchoa.html

[S14] C：枚举
来源：http://hz.xinyue.icu/gtjkjnzzdb.html


<!-- 参考信息 -->