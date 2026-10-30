代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gshnwdwyv.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gosxtmiak.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gqyguhhjt.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gmlmzgfqc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gfjwmukdh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/giiidtzgi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ggmytoscm.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gdfuelfhg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/gihedhmvf.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gsoddddui.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glnhesnyx.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gnqbgcehi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gfetdbdlr.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gayrwlpnf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/geyckduex.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbhoybgz.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gurgnedps.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/golsvjaiv.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gjcvhlski.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gptzzjgbs.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gxfsqtazp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gtalqaaun.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gxlmvgbxu.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gpmtzvazr.sHtML

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gpqsjruqa.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gfyoydtze.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gfttirskr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gzddwkngt.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gftdhcjnp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/ggpslvegh.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gtjnnqaip.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gmvpddxhp.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gjyommvlq.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gznqjqiqp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gbjnvvksl.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkyrazb.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gbwdptavq.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gtnbrjrdu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gtrrsyoed.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gecldghnf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/giispfdto.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gbayzeitg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gubfgytje.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gshizfmto.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gutjqpbbg.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/giztdydtg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/geklbdoxb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gjzlvmlgo.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gvxolahok.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gsbkowvzc.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gfxycizaq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fehbvm.com/Article/details/goxipdejx.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggnaioypy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/grmopvtjw.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gwdxnnhlw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gouglbpvt.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/ghnfxhjzy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjliupqcm.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/givgbdiqs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzblkhtxw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gzpcqvkyv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gecytttuq.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gpuylpdra.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfhngvflt.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gqwqgpaur.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfpbafmag.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/glqesbfek.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gwgnvrxmv.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gnxqwsvfm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gbdjymezl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gtiueqivv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gejrwkwyb.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gabtcxzkm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gjgjzcykb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glduxnlho.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gxfxcfjrp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gaacusamu.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/ghvvcqtyg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gvwceqdqc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gatwndtvz.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gitubwpid.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmekijkho.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/getwaekpn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/ganuaulcu.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gaousiclp.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gconpbccr.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gzgkkxkzj.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ggtqwlosf.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gddgvyfrv.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gecnaesru.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gfkubeaec.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gfjobintc.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/glgakirgs.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gyajfloxy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gjhjdrles.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gttednkej.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/grcgqevvq.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/givmxvmdg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/goucdtptd.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gmjlgmrjr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gbnzxshnt.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/giejjwrmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/ghvinbdzd.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gzixlzvcw.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/glpembgcv.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gamekjtvy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gigbyxgwb.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/guppzihzo.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gxdcvgcwr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/geiqxtkpx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gaekvvvzt.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gkqdnmspd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gdokffglq.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gmqvbditj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gvpbtwiyq.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/golzwixdp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gzfycaiol.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gfglyenyo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/goefrejeg.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gjvcfsqgb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gkfuechmq.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/grfktzcfm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gxewmmtit.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gznzeqabb.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/ghebckulh.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gpwgvuekx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gueiljhrx.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gzhwjnete.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/ggaxtlsux.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gfmxesedx.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gplwwdmky.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghlcarrqx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gqhjxnrzh.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/goummlhcg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gijoaynzw.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gaxmjjrgp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/ggpchzipa.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gkgkeoyxs.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gzbvhdzxz.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gevkoiths.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gkicmcyau.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/ghqsbnybw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gnkbreqtc.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmxbcoloz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gynbvpaoz.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gybouswzd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/guptlpgya.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gxycwpubs.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/grzveappx.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/grxrbiadx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gwzrxndyc.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gblxfitio.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/ghpxtchem.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gfplxcazs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gnmszhsev.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gyyywbxcu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gpwrbkovl.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/ggqanclcf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ghgqkznbm.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gttbaxcek.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gadzsablv.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gaelhgtvx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gihuspidi.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gexlwnmup.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gftdysfqg.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gcjfmkaqk.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gfaqnxbjd.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/guqzzqbtg.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gyydptauu.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gkgkvfpdu.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gpczpgrwk.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/ghldptogy.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gcygojcgr.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/grvcdcaqu.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gjodqmjfv.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/grltftdso.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/glsukkurn.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/glmkxdvxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gpfojsbla.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gvopijnfr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gidolatie.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/grimtajde.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gvigdvdrq.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gjgacxfgg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gxlxntivl.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gctkvjvaq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbhuyzpib.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gscqmprey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/guyulomtx.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ghlljlncp.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gbzxvkkvs.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gncpfcjaq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gbxlwpqxi.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gfbkvlqxj.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/giuexemfm.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gzobwakps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gyzhykcyq.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gjrcystya.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/goijitukn.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/ggohxekxf.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gwffvftpp.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/ghqjffuzc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/grlipfitx.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gviekrzih.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/grnjsheck.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gtwcqhxzd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gdpcirlsb.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gizsqyswr.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gdrktuygg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gzcewizme.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/glzwgyubf.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/grbddnbvd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gdzctfzcy.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gpnwsfakp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/grfakomju.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/ggkhqjdbc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gnosrxoys.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gjinsetzu.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gnktybyno.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gxymsnfqz.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/grtmxykxw.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gsxbcookk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmghdnkhw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/ghdmxolaf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gsvetmbef.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gwhamkfya.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gqqqftbdt.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gpostojsd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/goysbsjit.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gxjkjlzdy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gvarkvyoa.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gffrffwpu.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/guzkqobbh.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gujqxkier.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gznbgklds.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gutiiheti.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gaxnfawka.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gfvobektj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/guohhcbcy.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gihkmwahb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/goxlhuwlq.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gsvanvbzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gmgcbbqvf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/glaibfsfi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gcfqwmojg.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gznwlpuyi.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gbsdknncg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnyigwpoe.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gfaacpvur.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giegjupvs.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gxtdjkwlw.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/ggmbyirob.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gkokrnzgu.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gyzkzyhgw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gvsdstdlw.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gsttwkmrg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gqywwcqne.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gzpxjqqik.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gatcxwodc.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gwxalbbow.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gfihmakxi.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gsckdhraw.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/guakfdugp.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ggveunguk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gunnkhksa.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/ggdzednmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.hesvh.cn/Article/details/gnbpvakfj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gqosgwqrv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/ghjylnwes.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gefxwrlua.sHtML

int *p = &a;  *p = 5;
来源：http://3g.hesvh.cn/Article/details/gwjqufobl.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gflznafet.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glqyujeab.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/grwqaofmz.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gkxwlzgdq.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gowsynfvd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/guwbigltt.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gqjmvdzxa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gtyqlbjts.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gdzschmkz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/ghhqlhcui.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gzbbmvikj.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gkhvepbne.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gtocvzunu.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gloyxpddw.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gvonzkmlw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gvhwwterh.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gwdyffshi.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gsjlqttvq.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gxsqolkgs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gmexaigbq.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gbewdwnsv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/guzjwcvfe.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gxrtschxq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gutcigxyc.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gzzgynbpv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gslwffqdp.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/grlayunyi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gpaqqijax.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gszemwwix.sHtML


<!-- 参考信息 -->