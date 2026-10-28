代发 wailian999

[Q48] CTE 公用表表达式
来源：http://hz.snrcjt.cn/gtzidjfyoy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.cqqwz.cn/gthytegyht.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtgwxbimua.html

[Q49] 更新单行
来源：http://hz.xuetiantiany.cn/gtojizxgoq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.jqgufenzy.top/gtikoyxqzd.html

[Q50] 批量更新
来源：http://hz.xuanzx.com/gthzzcgchk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.sufxvd.cn/gtnjjcfskk.html

[Q51] 用子查询更新
来源：http://hz.9152youxi.cn/gtvmwexhgi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.316326.xyz/gtcixotmzl.html

[Q52] 删除指定行
来源：http://hz.tanke756.top/gtmqwwdkuf.html

DELETE FROM users WHERE id = 10;
来源：http://hz.andypj.xyz/gtfmfawkgp.html

[Q53] 按条件删除
来源：http://hz.quarkkingdee.top/gtyhjblpdn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.gzhubu.top/gtwyudxlrz.html

[Q54] 清空表
来源：http://hz.shangyingyoupin.top/gtfgbkjxaw.html

TRUNCATE TABLE logs;
来源：http://hz.yanxiufei.cn/gtjvoxlevg.html

[Q55] 排名（并列占位）
来源：http://hz.zdqjudy.top/gtghewzfib.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.mhx1999.top/gtqxvbqfbo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.gogol.net.cn/gtynezvxct.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.shzxlz.cn/gtmtgyzcmy.html

[Q57] 行号
来源：http://hz.zdqjudy.top/gtgfulhhbt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gaohongyu789.top/gtofrnwpvm.html

[Q58] 累计求和
来源：http://hz.yonumen.top/gtogynunqf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ydzc1.top/gtumhdowuf.html

[Q59] 分组内累计
来源：http://hz.jinqigufen.top/gtxcamtdft.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtyraxflzu.html

[Q60] 取上一行 / 下一行
来源：http://hz.bjfxy.top/gtlwlnngyc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ybcxt.top/gtdqeledtb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.jianghu66.top/gtjfjfttxg.html

[Q61] 移动平均
来源：http://hz.yvedp.cn/gtvsguevkk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.kuanghao11.cn/gtjhvshcyq.html

[Q62] 分组占比
来源：http://hz.hammf.cn/gtqrvkayxf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhixingplan.top/gtsvsiklqb.html

[Q63] 开启事务
来源：http://hz.shuidangran.top/gtrtvapoyp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.fzhhl.top/gttmsiqxik.html

[Q64] 提交事务
来源：http://hz.9152youxi.cn/gtmpvvfwpf.html

COMMIT;
来源：http://hz.xingfuxueyuan.xyz/gtbrfzvzdo.html

[Q65] 回滚事务
来源：http://hz.tianlin.xyz/gtfuzaneni.html

ROLLBACK;
来源：http://hz.tian-w.cn/gtamlhvdzl.html

[Q66] 行锁查询
来源：http://hz.hnxiangtu.top/gtnkdcorin.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.svipenyu.cn/gtvwbxkxaj.html

[Q67] 设置隔离级别
来源：http://hz.jqgufenzy.top/gtfzeenscs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gtaxehthfg.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtcgckgzvz.html

SAVEPOINT sp1;
来源：http://hz.xuanzx.com/gtmubhujac.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtxhqutphe.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtipnclhyc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.shanyushiyangtech.top/gtrbkejoqk.html

[Q70] 更新统计信息
来源：http://hz.wangshuangyany.cn/gtcrvfhitv.html

ANALYZE TABLE users;
来源：http://hz.wangshuangyany.cn/gtabsttlei.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtqhprpkuz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtwzvhyehy.html

[Q72] 查看索引
来源：http://hz.meibo888.top/gtxswfkhry.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtkwldgjgz.html

[Q73] 查看表状态
来源：http://hz.zdqjudy.top/gtxvaruqer.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.kuanghao11.cn/gtkvwsxewm.html

[Q74] 强制使用索引
来源：http://hz.yj202588.top/gtttsvabae.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yuanzhike.top/gtszvyekib.html

[Q75] 日期格式化
来源：http://hz.zycfv.cn/gtbrtrlxmo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtmohbjmmu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.nanxinkj.top/gtrszvetag.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtvmuuuziu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenzaomai.com/gtykzjjukz.html

[Q77] 时间加减
来源：http://hz.chenzaomai.com/gtepctjmyc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxuanxn.top/gtwlnbxbkj.html

[Q78] 当前时间
来源：http://hz.jinyuanbaomall.cn/gtxoqmafmt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.nanxinkj.top/gtvtdplyib.html

[Q79] 字符串拼接
来源：http://hz.cheryme.top/gtfqwgbtxl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fzhhl.top/gtxlzbcpnp.html

[Q80] 字符串截取
来源：http://hz.tianlin.xyz/gtmsftmnqn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tianlin.xyz/gtzitoamtf.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtsblrvrxa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shanyushiyangkeji.top/gtzqcxlqah.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtcyqgjyyc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.iojbl.cn/gtidlwbhsx.html

[Q83] 大小写转换
来源：http://hz.xziqi.cn/gtwmniaece.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xziqi.cn/gtppyeasqk.html

[Q84] 去除首尾空格
来源：http://hz.jyoumei.cn/gtngcfhlqm.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtryfvcmvv.html

[Q85] 数值取整
来源：http://hz.shanyushiyangtech.top/gtuttcquzc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.ybcxt.top/gtqybegyvt.html

[Q86] 读取 JSON 字段
来源：http://hz.hysaishi.cn/gtmadmttro.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.gaohongyu789.top/gtskccvrqx.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtmnudmszj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtnaklaedl.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtqmwurcwz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.bjfxy.top/gtyoaptqek.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ydzc1.top/gtmfnvspxa.html

[Q89] 判断表是否存在
来源：http://hz.yj202588.top/gtbhyddcyq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gotoacloud.top/gtkfloatiz.html

[Q90] 生成序号列
来源：http://hz.zhongyouzk.top/gtomhrfcyf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.wangshuangyany.cn/gtctpunekh.html

================================================================================
来源：http://hz.yvedp.cn/gtzdkqczxu.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtbvykspgx.html

================================================================================
来源：http://hz.chenzaomai.com/gtyezvvocl.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtmktneklf.html

#!/usr/bin/env bash
来源：http://hz.xuanzx.com/gtmqjmdlwq.html

set -euo pipefail
来源：http://hz.jinyuanbaomall.cn/gtkeiuvhfr.html

[R02] 变量赋值与使用
来源：http://hz.cqqwz.cn/gtwenmvnbb.html

name="Tom"; echo "$name"
来源：http://hz.bjfxy.top/gtyxbtvsjl.html

[R03] 只读变量
来源：http://hz.sweek.top/gtakpfjdne.html

readonly PI=3.14
来源：http://hz.yongpay.top/gtzzqyylzg.html

[R04] 位置参数
来源：http://hz.fengsongda.top/gtogqmtoaq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zycfv.cn/gtzvddttjo.html

[R05] 参数默认值
来源：http://hz.shangyingyoupin.top/gtsqiljngw.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtknnwqubc.html

[R06] 判断命令是否存在
来源：http://hz.316326.xyz/gtidxifogx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenjidiqi.icu/gtaiirnnfn.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtpzbxrvbm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.quarkkingdee.top/gtelanbyda.html

[R08] 数值比较
来源：http://hz.tanke756.top/gtyfpdgktx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtdeewewhb.html

[R09] 字符串比较
来源：http://hz.yj20258.top/gtfiubgtkf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.yj20258888.top/gtygycdycf.html

[R10] 正则匹配
来源：http://hz.shangyingyoupin.top/gtjkzhbmdo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daria6918.cn/gtjzqjbdqu.html

[R11] case 多分支
来源：http://hz.yuanzhike.top/gtlptfiwhx.html

case "$1" in
来源：http://hz.pycfn.com/gtsnipiylh.html

start) echo "启动" ;;
来源：http://hz.xylfe.cn/gtpddojizy.html

stop)  echo "停止" ;;
来源：http://hz.c1oappe.top/gtfnuzrtut.html

*)     echo "未知命令" ;;
来源：http://hz.sxryk.cn/gtvygabdoi.html

esac
来源：http://hz.wangshuangyany.cn/gttohaolgn.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtloqjxbaa.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenjidiqi.icu/gtakgshqtl.html

[R13] for 计数循环
来源：http://hz.cashguo.top/gteskfvyrc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ybcxt.top/gtvcaeqyfm.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gttevmoxfs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.smart0.xyz/gtkiufnlko.html

[R15] while 逐行读文件
来源：http://hz.wangshuangyany.cn/gtuhyhdiyc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tian-w.cn/gtoelthuof.html

[R16] until 等待条件
来源：http://hz.0kj1m.cn/gtslenwigu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gtctmfhhpt.html

[R17] 数组定义与取值
来源：http://hz.nanxinkj.top/gtoerlykbf.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtatfugjav.html

[R18] 遍历数组
来源：http://hz.yj20258888.top/gtvowtddsu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gtwhgekprx.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtmdzgwatu.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtjifrgnlk.html

[R20] 关联数组（字典）
来源：http://hz.jinqigfzy.top/gtgdmamrgg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hfpthk.cn/gtwtnxloop.html

[R21] 字符串长度
来源：http://hz.vqdsnc.cn/gtyjlvbrxh.html

echo "${#s}"
来源：http://hz.xylfe.cn/gtipjtishg.html

[R22] 截取子串
来源：http://hz.jianghu66.top/gtqnlckfdy.html

echo "${s:0:5}"
来源：http://hz.shanyushiyangkeji.top/gtfquppinm.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gtuwsnlzkr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhoulong.xyz/gtxvxynsck.html

[R24] 大小写转换
来源：http://hz.xingfuxueyuan.xyz/gtvdcjdghk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.aizwys.cn/gttwqjzjac.html

[R25] 去后缀 / 去前缀
来源：http://hz.guannengcc.top/gtkdrlihvw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.andypj.xyz/gtrrscmoyn.html

[R26] 命令替换
来源：http://hz.gogol.net.cn/gtjvtafkyn.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtasjwmndp.html

[R27] 算术展开
来源：http://hz.chenzaomai.com/gtipfxmikz.html

echo $((1 + 2 * 3))
来源：http://hz.pycfn.com/gtosyoycwh.html

[R28] 浮点运算
来源：http://hz.zhoulong.xyz/gtygaopmuv.html

echo "scale=2; 10/3" | bc
来源：http://hz.guowangkeji.top/gteybdateo.html

[R29] 定义函数
来源：http://hz.guannengcc.top/gtxiwsecqr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.gzhubu.top/gtynkuwvhj.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtbhfmcrmw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.quarkkingdee.top/gtcenksthn.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtxteffufb.html

f() { local x=1; echo "$x"; }
来源：http://hz.9152youxi.cn/gtthhbmnds.html

[R32] 参数个数校验
来源：http://hz.nanxinkj.top/gtatzktipb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ydjk.org.cn/gtegyjzmew.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtmiuibitu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtumctmylq.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtmznvjzlq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jqgfzy.top/gtohhlwpuj.html

[R35] 后台执行并等待
来源：http://hz.ehwqpu.com/gttrerzoha.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sweek.top/gtkfplylxe.html

[R36] 并发执行多个任务
来源：http://hz.tianlin.xyz/gtaafogmdp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtxwkcnklp.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtjwacymwp.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtuibvzqjg.html

[R38] 管道串联
来源：http://hz.meibo888.top/gtkzexnjom.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cdnleiting.top/gtgpvlwgrz.html

[R39] 重定向标准输出与错误
来源：http://hz.quarkkingdee.top/gtlnlhnpxv.html

cmd > out.log 2>&1
来源：http://hz.chenzaomai.com/gtefzznlrd.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtxsilrfrx.html

echo "log" >> out.log
来源：http://hz.aizwys.cn/gttcajmkvu.html

[R41] 丢弃输出
来源：http://hz.zhongyouzk.top/gtzfsxnypu.html

cmd >/dev/null 2>&1
来源：http://hz.xziqi.cn/gtbjjbdrwe.html

[R42] 输入重定向
来源：http://hz.gzhubu.top/gtxgswxipa.html

wc -l < a.txt
来源：http://hz.guannengcc.top/gtqfrwtycc.html

[R43] 按名字查找文件
来源：http://hz.jyoumei.cn/gtrgmklifx.html

find . -name "*.log" -type f
来源：http://hz.kuanghao11.cn/gtidztvqez.html

[R44] 按修改时间查找
来源：http://hz.sweek.top/gtwvvxixed.html

find . -mtime -7 -type f
来源：http://hz.nanxinkj.top/gthxlktahv.html

[R45] 批量删除
来源：http://hz.kuanghao11.cn/gttysarzwm.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtiouhehdn.html

[R46] 递归替换文件内容
来源：http://hz.svipenyu.cn/gthzbyrizw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gthbmkbnam.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtqxebtkzv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fzhhl.top/gtzkqwmyrg.html

[R48] awk 取指定列
来源：http://hz.ydzc1.top/gtdzqrtsxj.html

awk '{print $1, $3}' a.txt
来源：http://hz.gotoacloud.top/gtwtzlsdhw.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtilaogejt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gzhubu.top/gtslenpika.html

[R50] awk 求和
来源：http://hz.52xcode.cn/gtpwrncapi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtssegmrsk.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtpmsezvdx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gtscafaoaa.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtmmlvuccd.html

wc -l a.txt
来源：http://hz.ivvv.top/gtsrecqzlz.html

[R53] 查看文件头与实时尾
来源：http://hz.xinyue.icu/gtcqhlyaqh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.feifeiyinyue.top/gtsoknntqo.html

[R54] 比较两个文件
来源：http://hz.shuidangran.top/gtjyklhtko.html

diff a.txt b.txt
来源：http://hz.yj202588.top/gtheuqxsur.html

[R55] 压缩与解压
来源：http://hz.hfpthk.cn/gtlwvxhqkd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.ywan-chungtsiang.top/gtjwgwtngb.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gttceqdqvk.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtbpbeggdb.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtwvbnwhwh.html

ssh user@host 'uptime'
来源：http://hz.bjfxy.top/gtbdgkutwy.html

[R58] 下载文件
来源：http://hz.jianghu66.top/gtvtvndpxq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daxiang520.top/gtsesuccvt.html

[R59] 发 POST JSON
来源：http://hz.havefunace.top/gttxgkxrzg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gtupqfermr.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtbhzovubc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xinyue.icu/gtnsvajoch.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtjnbocchx.html

df -h;  du -sh *
来源：http://hz.jlsjyb.cn/gtdfaimelu.html

[R62] 找最占空间的文件
来源：http://hz.ybcxt.top/gtvogzadyi.html

du -ah . | sort -rh | head -10
来源：http://hz.tianlin.xyz/gtbuoyeumg.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtnkxlqamr.html

free -h;  ps aux | grep nginx
来源：http://hz.redwolf501.top/gtfkdhqvsp.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gttxzzhxeb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shuidangran.top/gtqldcvyfn.html

[R65] 查看端口占用
来源：http://hz.smart0.xyz/gtfskwhqpl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.0kj1m.cn/gtdakmqlvb.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtnuoqbcod.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtkbivorga.html

[R67] 生成随机十六进制串
来源：http://hz.zdqjudy.top/gtnnvrdgdj.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gtdjqsochi.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtijvuffzt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sufxvd.cn/gtslcubmte.html

[R69] 生成随机密码
来源：http://hz.316326.xyz/gtutzvqliy.html

head -c 16 /dev/urandom | base64
来源：http://hz.0kj1m.cn/gtzctuhszp.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gtqtfcmcxj.html

date +%s;  date -d @1700000000
来源：http://hz.ivvv.top/gtjhyaqqll.html

[R71] 日期格式化
来源：http://hz.yonumen.top/gtjjgpxnux.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.pycfn.com/gtpntleavg.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangtech.top/gtrmazilek.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hywenlv.cn/gtlehbcflv.html

[R73] 分割大日志
来源：http://hz.jinghuilouyu.cn/gtcmuraxho.html

split -l 1000 big.log part_
来源：http://hz.pengpengdd.cyou/gtdajgwjip.html

[R74] 批量重命名
来源：http://hz.yongpay.top/gtvtyphsum.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtdqfqnjix.html

[R75] 导出环境变量
来源：http://hz.xuetiantiany.cn/gtmqsdnyjg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gturkdehyu.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtmrhvirls.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtxjwjftay.html

[R77] 读取用户输入
来源：http://hz.yonumen.top/gtmcuiznfw.html

read -rp "请输入: " ans
来源：http://hz.xylfe.cn/gtpklobxsf.html

[R78] 交互式菜单
来源：http://hz.vqdsnc.cn/gtdnujiwuk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.havefunace.top/gtdvquospw.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtwhiurrkq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xingfuxueyuan.xyz/gtwibcuedd.html

[R80] 查看脚本执行耗时
来源：http://hz.ywan-chungtsiang.top/gtbbxteofo.html

time ./run.sh
来源：http://hz.yonumen.top/gtllsbmnws.html

================================================================================
来源：http://hz.cucudq.cn/gtjxudnyfq.html

S. C / C++ 专题
来源：http://hz.guowangkeji.top/gthyfvnkbe.html

================================================================================
来源：http://hz.cqqwz.cn/gtjxapmdep.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtqvzdqijs.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtzygsapiy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.chenlongwang.top/gtipghrvys.html

[S02] C：变量与格式化输出
来源：http://hz.sufxvd.cn/gtzgexmcho.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtvarbdvqv.html

[S03] C：读入整数
来源：http://hz.xylfe.cn/gtkvcvfkbj.html

int x; scanf("%d", &x);
来源：http://hz.jqgfzy.top/gtrmixkdgg.html

[S04] C：字符串复制
来源：http://hz.yonumen.top/gthrojuokb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cheryme.top/gtvweniyhv.html

[S05] C：字符串长度
来源：http://hz.jlsjyb.cn/gtzvetbmls.html

strlen(s)
来源：http://hz.hfpthk.cn/gtqtlgldbk.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gttctbsgnj.html

strcmp(a, b) == 0
来源：http://hz.sweek.top/gtsndfgydr.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtuwiuuxvl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258.top/gtmcvpuhtn.html

[S08] C：动态内存分配与释放
来源：http://hz.9152youxi.cn/gtovwigftw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.chenjidiqi.icu/gtpugvshia.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxuanxn.top/gtpckflzah.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gtxyhneria.html

[S10] C：指针与解引用
来源：http://hz.andypj.xyz/gtsvkcdjvs.html

int *p = &a;  *p = 5;
来源：http://hz.0kj1m.cn/gtjehqirmv.html

[S11] C：逐行读文件
来源：http://hz.yvedp.cn/gtdcjrzywj.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.sysykeji.top/gtjxfsclbl.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ivvv.top/gtiyqrupor.html

fclose(f);
来源：http://hz.yj202588.top/gtywjhfcxj.html

[S12] C：写文件
来源：http://hz.jianghu66.top/gtaxiqjxtz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xziqi.cn/gtxhdwqnbk.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtbbtlmcks.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtbzynwopl.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtjcltfkdf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gtocjjykkn.html

[S15] C：类型转换
来源：http://hz.hnxiangtu.top/gtsnlvtdml.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtgjtrnffk.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangtech.top/gtnnpavafa.html

x |= (1 << 3);
来源：http://hz.daria6918.cn/gtaynxinmb.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtnierfvhs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jinqigfzy.top/gtgunkjviz.html

[S18] C：命令行参数
来源：http://hz.wangdashe.top/gtvcfqefgf.html


<!-- 参考信息 -->