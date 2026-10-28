代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://hz.yonumen.top/gtbaxiuigd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.jianghu66.top/gtmfvpnabs.html

[Q47] 与平均值比较
来源：http://hz.yuxming.cn/gtqdbwffko.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.jqgufenzy.top/gtppobafcp.html

[Q48] CTE 公用表表达式
来源：http://hz.sysykeji.top/gtjvfqbqep.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ppjwa.cn/gtvddiaxna.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.andypj.xyz/gtocdunpjz.html

[Q49] 更新单行
来源：http://hz.daxiang520.top/gtnkbdoqjf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.kuanghao11.cn/gtrsofbheu.html

[Q50] 批量更新
来源：http://hz.c1oappe.top/gthmuebgny.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.gaohongyu789.top/gtucgjjenj.html

[Q51] 用子查询更新
来源：http://hz.havefunace.top/gtfutsrfwq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.c1oappe.top/gtljekyuwu.html

[Q52] 删除指定行
来源：http://hz.xuetiantiany.cn/gtqtwbslsh.html

DELETE FROM users WHERE id = 10;
来源：http://hz.jlsjyb.cn/gtyvpnfcqb.html

[Q53] 按条件删除
来源：http://hz.jinqigfzy.top/gtisfvfnyp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.316326.xyz/gtbhzngnte.html

[Q54] 清空表
来源：http://hz.zhijiandao.cn/gtcqpywbmi.html

TRUNCATE TABLE logs;
来源：http://hz.zycfv.cn/gtxnvkbhss.html

[Q55] 排名（并列占位）
来源：http://hz.yueranfly.top/gtqswyznwb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.andypj.xyz/gtujgaukqj.html

[Q56] 密集排名（并列不占位）
来源：http://hz.vqdsnc.cn/gtslaukwqs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.fzhhl.top/gtjvfkgtut.html

[Q57] 行号
来源：http://hz.shanyushiyangkeji.top/gtxqcklcab.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtmjbwgyvl.html

[Q58] 累计求和
来源：http://hz.sxryk.cn/gteyweoisn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.havefunace.top/gtthbrxhqy.html

[Q59] 分组内累计
来源：http://hz.dianchejie.cn/gtjqbcplps.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.meibo888.top/gtpmbxbtpt.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhaomingkeji.xyz/gtgjingwoi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.vqdsnc.cn/gtgefzvjxr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fzhhl.top/gtsnpuqwkv.html

[Q61] 移动平均
来源：http://hz.hammf.cn/gtjrmahohu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtnbcqeypa.html

[Q62] 分组占比
来源：http://hz.xuanzx.com/gtoxrspwzb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.bjfxy.top/gtbyujmbso.html

[Q63] 开启事务
来源：http://hz.quarkkingdee.top/gtgaejscio.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.tanke756.top/gtaokakzry.html

[Q64] 提交事务
来源：http://hz.pengpengdd.cyou/gttxygiooe.html

COMMIT;
来源：http://hz.nwbrower.top/gtqoowgyih.html

[Q65] 回滚事务
来源：http://hz.shuidangran.top/gtmisnftbz.html

ROLLBACK;
来源：http://hz.yvedp.cn/gtezktrkgh.html

[Q66] 行锁查询
来源：http://hz.feifeiyinyue.top/gtefnbjozt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.guannengcc.top/gtovskdiso.html

[Q67] 设置隔离级别
来源：http://hz.guowangkeji.top/gtwfrrkeao.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.shanyushiyangtech.top/gtxbizxhwv.html

[Q68] 保存点
来源：http://hz.hysaishi.cn/gteoahqfar.html

SAVEPOINT sp1;
来源：http://hz.pycfn.com/gtwrpgrwqh.html

ROLLBACK TO sp1;
来源：http://hz.yangfankeji.com/gtekmofzpn.html

[Q69] 查看执行计划
来源：http://hz.ehwqpu.com/gtbuohikhd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.snrcjt.cn/gtnvbrrnix.html

[Q70] 更新统计信息
来源：http://hz.ydjk.org.cn/gtgxgkewqs.html

ANALYZE TABLE users;
来源：http://hz.jlsjyb.cn/gtgepxpiot.html

[Q71] 查看建表语句
来源：http://hz.yj202588.top/gtlgxolxis.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinghuilouyu.cn/gtdgvqzstr.html

[Q72] 查看索引
来源：http://hz.vqdsnc.cn/gtjzpvibbf.html

SHOW INDEX FROM users;
来源：http://hz.birdmap.top/gtgwnamwmr.html

[Q73] 查看表状态
来源：http://hz.shzxlz.cn/gtqdusfnyc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.meibo888.top/gtkeeuydcg.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtngnuaebe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.havefunace.top/gturdzrdyz.html

[Q75] 日期格式化
来源：http://hz.aibaodan.cn/gtbepfuisl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.jlsjyb.cn/gtyxlxeddg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.gzhubu.top/gtoflxpxkj.html

[Q76] 按天统计
来源：http://hz.cdnleiting.top/gtizynfsxg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.aizwys.cn/gtorbxzuxv.html

[Q77] 时间加减
来源：http://hz.dianchejie.cn/gtyexcfhzy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtzswbydva.html

[Q78] 当前时间
来源：http://hz.xuetiantiany.cn/gtrkenchjj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.snrcjt.cn/gtkvpqunka.html

[Q79] 字符串拼接
来源：http://hz.vqdsnc.cn/gtfhqswrly.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.redwolf501.top/gtuhtypfrq.html

[Q80] 字符串截取
来源：http://hz.sysykeji.top/gtvfmnsfuj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.nanxinkj.top/gtpabspjhk.html

[Q81] 字符串替换
来源：http://hz.sufxvd.cn/gtddqjjljb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.ydjk.org.cn/gtmlyhqlun.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtcklovlzf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gteploymif.html

[Q83] 大小写转换
来源：http://hz.tanke756.top/gtbkauytdb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtlozokcsn.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gttyoamgrn.html

SELECT TRIM(name) FROM users;
来源：http://hz.shuidangran.top/gtgtjvxmyo.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gtjlegwttw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.dianchejie.cn/gtbktkdvsk.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtewblmkvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.hysaishi.cn/gtkpiskoni.html

[Q87] JSON 字段做条件
来源：http://hz.shangyingyoupin.top/gttwrpjwcd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.kuanghao11.cn/gtxdvxuoxq.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtiebrzdwf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cqqwz.cn/gtenhdernn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.kuanghao11.cn/gtfemxdunh.html

[Q89] 判断表是否存在
来源：http://hz.jinyuanbaomall.cn/gtpfpdmhbz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.aibaodan.cn/gtdaavntrt.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtvkvfbuao.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.hywenlv.cn/gtkuoehqnn.html

================================================================================
来源：http://hz.nanxuanxn.top/gtlckawvuc.html

R. Bash 专题
来源：http://hz.shangyingyoupin.top/gtcoyhwncv.html

================================================================================
来源：http://hz.tianlin.xyz/gtvyjmeuup.html

[R01] shebang 与严格模式
来源：http://hz.ehwqpu.com/gtsrkkhwcv.html

#!/usr/bin/env bash
来源：http://hz.cqqwz.cn/gtvmmwgefu.html

set -euo pipefail
来源：http://hz.pengpengdd.cyou/gtflmogszk.html

[R02] 变量赋值与使用
来源：http://hz.havefunace.top/gtjenczgjz.html

name="Tom"; echo "$name"
来源：http://hz.wangdashe.top/gtebnnyauu.html

[R03] 只读变量
来源：http://hz.yongpay.top/gtnzrhyolz.html

readonly PI=3.14
来源：http://hz.tanke756.top/gthsfvgwcm.html

[R04] 位置参数
来源：http://hz.nanxinkj.top/gtxfzbyweu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.52xcode.cn/gttpantotp.html

[R05] 参数默认值
来源：http://hz.svipenyu.cn/gtinvtlmxh.html

name="${1:-default}"
来源：http://hz.mhx1999.top/gtleikjhmn.html

[R06] 判断命令是否存在
来源：http://hz.yuxming.cn/gtitfelfbo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nwbrower.top/gttlwdsgyo.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtyfibyjwp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtlhzajsxn.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gtqhtroamp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ydjk.org.cn/gtgsviezxb.html

[R09] 字符串比较
来源：http://hz.cqqwz.cn/gtzqbvalhv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gogol.net.cn/gteefvsanx.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtpyimfshv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtxretwfha.html

[R11] case 多分支
来源：http://hz.gzhubu.top/gtvhwbcgov.html

case "$1" in
来源：http://hz.aibaodan.cn/gtnlxznwts.html

start) echo "启动" ;;
来源：http://hz.guannengcc.top/gtxmdbzsqt.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtvyctvgjb.html

*)     echo "未知命令" ;;
来源：http://hz.guannengcc.top/gtbeaayyyo.html

esac
来源：http://hz.shanyushiyangtech.top/gtrhzefvcu.html

[R12] for 遍历文件
来源：http://hz.wangdashe.top/gtmwtegqgc.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yj20258.top/gtjbdqcjxl.html

[R13] for 计数循环
来源：http://hz.redwolf501.top/gtbtegorry.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gogol.net.cn/gtngayxcbz.html

[R14] C 风格 for
来源：http://hz.yanxiufei.cn/gttoeuivad.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.chenlongwang.top/gtnaspuzrq.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtdvezixyw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtxewfjacq.html

[R16] until 等待条件
来源：http://hz.daria6918.cn/gtdciivyjg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtrmuatven.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtrisvxsnw.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenjidiqi.icu/gtrogeggtr.html

[R18] 遍历数组
来源：http://hz.havefunace.top/gtefujikze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fzhhl.top/gtgvodeyoe.html

[R19] 数组长度
来源：http://hz.nwbrower.top/gtmosohack.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtltrkshdq.html

[R20] 关联数组（字典）
来源：http://hz.zhongyouzk.top/gtynrreumu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinqigfzy.top/gtcewsylar.html

[R21] 字符串长度
来源：http://hz.nanxuanxn.top/gtlkhhohdw.html

echo "${#s}"
来源：http://hz.jyoumei.cn/gtcpzbccqa.html

[R22] 截取子串
来源：http://hz.jqgufenzy.top/gtebyydeld.html

echo "${s:0:5}"
来源：http://hz.yj202588.top/gtoehnjhhr.html

[R23] 字符串替换
来源：http://hz.zhongyouzk.top/gtyudynaku.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhongyouzk.top/gtucfrbzpp.html

[R24] 大小写转换
来源：http://hz.pycfn.com/gtaeluznwm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ywan-chungtsiang.top/gtmxzeuzgt.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtjdynczvs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.daxiang520.top/gtnckkhccd.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtptbfkksa.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gtfjbbyvnx.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtqohyaydq.html

echo $((1 + 2 * 3))
来源：http://hz.sysykeji.top/gtyjhrundg.html

[R28] 浮点运算
来源：http://hz.316326.xyz/gtvulqqmnf.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtxsadweqi.html

[R29] 定义函数
来源：http://hz.ehwqpu.com/gthevsfqps.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gtcnwhyayl.html

[R30] 函数返回状态码
来源：http://hz.fengsongda.top/gthbpjhlhd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtjhokmswz.html

[R31] 局部变量
来源：http://hz.sxryk.cn/gtpeecwipb.html

f() { local x=1; echo "$x"; }
来源：http://hz.cdnleiting.top/gtwenlhkob.html

[R32] 参数个数校验
来源：http://hz.yvedp.cn/gtlvomucgs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gtvbhrhhzl.html

[R33] 捕获错误并提示行号
来源：http://hz.ydjk.org.cn/gtcyiwhoth.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gogol.net.cn/gtrxhvfaau.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gtiqgjezwl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.c1oappe.top/gtqkrmdztr.html

[R35] 后台执行并等待
来源：http://hz.chenlongwang.top/gtpewkizbo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zdqjudy.top/gtbofttbyl.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtlrmmxhhl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.bjfxy.top/gtmunpwbmf.html

[R37] 把输出赋给变量
来源：http://hz.c1oappe.top/gtknxnpjdp.html

files=$(ls -1)
来源：http://hz.xingfuxueyuan.xyz/gtotsmmaxo.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtjrtqtxez.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yvedp.cn/gtrajijpjo.html

[R39] 重定向标准输出与错误
来源：http://hz.9152youxi.cn/gtulmfchbh.html

cmd > out.log 2>&1
来源：http://hz.yangfankeji.com/gtusxtaqdv.html

[R40] 追加写日志
来源：http://hz.meibo888.top/gtsjalakkp.html

echo "log" >> out.log
来源：http://hz.hongshengwenyu.top/gtdtpqjnpf.html

[R41] 丢弃输出
来源：http://hz.zycfv.cn/gtzbvsqeuv.html

cmd >/dev/null 2>&1
来源：http://hz.nwbrower.top/gtytayjbao.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gttvfmedtr.html

wc -l < a.txt
来源：http://hz.mhx1999.top/gtcyupapel.html

[R43] 按名字查找文件
来源：http://hz.haohaochexian.top/gtsvqodjgh.html

find . -name "*.log" -type f
来源：http://hz.vqdsnc.cn/gtdilqgmtk.html

[R44] 按修改时间查找
来源：http://hz.yj20258888.top/gtpfrukuxm.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtaijbiqqb.html

[R45] 批量删除
来源：http://hz.meibo888.top/gtvvkjvjdn.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtmhdvgnwo.html

[R46] 递归替换文件内容
来源：http://hz.cqqwz.cn/gtkckcniyb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hnqzz.top/gtqxfoaiwo.html

[R47] sed 单行替换
来源：http://hz.yj202588.top/gtbjntvfij.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangtech.top/gtbshudkfn.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtubwgodzm.html

awk '{print $1, $3}' a.txt
来源：http://hz.ydzc1.top/gtdgdktoxz.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtgvwlhheq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.fzhhl.top/gtszwdyozy.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gtueugjflv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtyqkdyjqn.html

[R51] 排序去重取前几
来源：http://hz.chenzaomai.com/gtafynrvsx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jyoumei.cn/gtntnhzlkl.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtdaaudzpu.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtlsvootho.html

[R53] 查看文件头与实时尾
来源：http://hz.316326.xyz/gtijuqkdcy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.vqdsnc.cn/gtsbzjlwlq.html

[R54] 比较两个文件
来源：http://hz.xuetiantiany.cn/gtjrrsqqxt.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtvhzmexfr.html

[R55] 压缩与解压
来源：http://hz.cucudq.cn/gttvmxdrsz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daxiang520.top/gtpvespevo.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtevphzanr.html

scp file user@host:/path/
来源：http://hz.xuanzx.com/gtagjmqiny.html

[R57] 远程执行命令
来源：http://hz.ybcxt.top/gtvyazixkr.html

ssh user@host 'uptime'
来源：http://hz.ybcxt.top/gtqbtixowp.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtziftgmda.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.feifeiyinyue.top/gtowovixsh.html

[R59] 发 POST JSON
来源：http://hz.cqqwz.cn/gtbafkfsea.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gotoacloud.top/gtcxnnqdao.html

[R60] 只看 HTTP 状态码
来源：http://hz.nwbrower.top/gtnroxpptf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gthhwbwtzy.html

[R61] 磁盘占用
来源：http://hz.nwbrower.top/gtojcolppl.html

df -h;  du -sh *
来源：http://hz.tanke756.top/gtaxtkepio.html

[R62] 找最占空间的文件
来源：http://hz.yj20258888.top/gtqbkzogio.html

du -ah . | sort -rh | head -10
来源：http://hz.mhx1999.top/gtmbyzwytc.html

[R63] 内存与进程
来源：http://hz.shuidangran.top/gtramvpscm.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtzajfhuhc.html

[R64] 结束进程
来源：http://hz.zhixingplan.top/gtrzywtayq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinghuilouyu.cn/gtmxfvfdlq.html

[R65] 查看端口占用
来源：http://hz.52xcode.cn/gtdzlziaeq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.kuanghao11.cn/gtafutwaqc.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gtximdrjge.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtpgxaesjl.html

[R67] 生成随机十六进制串
来源：http://hz.shanyushiyangkeji.top/gtifkfhvbq.html

openssl rand -hex 16
来源：http://hz.ywan-chungtsiang.top/gtorspmmnu.html

[R68] 计算文件校验值
来源：http://hz.yongpay.top/gthhghcwbo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aizwys.cn/gtpbvdhxkf.html

[R69] 生成随机密码
来源：http://hz.gzhubu.top/gtlohnkknk.html

head -c 16 /dev/urandom | base64
来源：http://hz.pycfn.com/gtovvipxze.html

[R70] 时间戳与互转
来源：http://hz.yuanzhike.top/gtmdjaszgv.html

date +%s;  date -d @1700000000
来源：http://hz.guowangkeji.top/gtccghbgqw.html

[R71] 日期格式化
来源：http://hz.52xcode.cn/gtwszuduob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yonumen.top/gtjjsfggio.html

[R72] 等待端口就绪
来源：http://hz.xuanzx.com/gtgojodboc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtvkzoeqia.html

[R73] 分割大日志
来源：http://hz.hywenlv.cn/gtsmcomocr.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtxuixroxr.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtrcviqmiq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.bjfxy.top/gtjychitet.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gtjsbkmspm.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jianghu66.top/gtlqkzumvl.html

[R76] 使用临时文件
来源：http://hz.smart0.xyz/gtpmardytc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtcfibyyse.html

[R77] 读取用户输入
来源：http://hz.yanxiufei.cn/gtlysufrkb.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gtxxanzldp.html

[R78] 交互式菜单
来源：http://hz.sufxvd.cn/gtiaenwrye.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ppjwa.cn/gtocyxyepx.html

[R79] 解析命令行选项
来源：http://hz.yueranfly.top/gtwepiqwby.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.haohaochexian.top/gtmogodqqg.html

[R80] 查看脚本执行耗时
来源：http://hz.yongpay.top/gtaflphvve.html

time ./run.sh
来源：http://hz.aizwys.cn/gttjqjaqkc.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpwkyqanz.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtugcpfubz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtuuypkiqj.html

[S01] C：Hello World
来源：http://hz.chenlongwang.top/gthcundefm.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtafkcfugf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtcnfqwaem.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtccoxefvb.html

int a = 10; printf("%d\n", a);
来源：http://hz.jyoumei.cn/gtmpkcgeef.html

[S03] C：读入整数
来源：http://hz.yueranfly.top/gtagevclyu.html

int x; scanf("%d", &x);
来源：http://hz.xinyue.icu/gtbspyvsih.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtutgfnsqs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gtpoevpwvt.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtjcwmiijm.html

strlen(s)
来源：http://hz.hysaishi.cn/gtcgfchkcb.html

[S06] C：字符串比较
来源：http://hz.jinyuanbaomall.cn/gtfdzbwdcr.html

strcmp(a, b) == 0
来源：http://hz.gogol.net.cn/gtsxlraaus.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtdmgekpqp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jyoumei.cn/gtrdckjjjj.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtzmlzslwk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dianchejie.cn/gtudwylkpo.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtpbjrbaie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yongpay.top/gtlmreqemg.html

[S10] C：指针与解引用
来源：http://hz.bjfxy.top/gtlvtbeqic.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtnkrrhaau.html

[S11] C：逐行读文件
来源：http://hz.cucudq.cn/gtkwgljayg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hywenlv.cn/gtxaqujmnv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtwdtgfkme.html

fclose(f);
来源：http://hz.hywenlv.cn/gtxilsrvgy.html

[S12] C：写文件
来源：http://hz.yonumen.top/gtdmuuqhut.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gtctmqrjxi.html

[S13] C：宏定义
来源：http://hz.aizwys.cn/gtpuvtdrfa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hywenlv.cn/gtpozjxkmc.html

[S14] C：枚举
来源：http://hz.hfpthk.cn/gtklfvnixj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydjk.org.cn/gtrntuavgh.html

[S15] C：类型转换
来源：http://hz.cashguo.top/gtqvcjikye.html

(double) a / b
来源：http://hz.xziqi.cn/gtmdreeyyp.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtjgkeeinm.html


<!-- 参考信息 -->