代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gdiwexihr.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gangwfxng.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gbibedvmf.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/goxzisqob.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gxiyvraps.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gbvxoliwt.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gcnqdeggo.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxckfqaxu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/grczibifm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/grbwinqlz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gidbvaovm.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gsvacgsbd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gothlibyo.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gtrmircrw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gztpdgfgt.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gasxnwzul.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gnjabetjv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gevhuxqak.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gwtutdrsz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdaztowkf.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gcdmhjhrx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gldnabpnf.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/ggysdqzpe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gkgsgwjml.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gbzbmcnor.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/goxuxxxvg.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/goaebvbqo.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gpumardoz.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gyxifzgcc.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gvirmnwmq.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gqcednnrx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gpxyszdcj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gliewjlyu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gxoooqfrq.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gvrpjzlux.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdeczzgwt.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gnozdeirq.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gqzqiovcj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/glsbhdkyg.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gaerlzzid.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gdvmrszfs.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/geqiieraw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/guqfrysjp.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gbjvresdy.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gazoxmxzd.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/grfbddlpz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gyddesohk.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gixreohon.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/glljqodhf.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gpxlfkyeo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxefsbhxh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gskhwzhiw.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gvkognlsk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gotmeokdj.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/ghcejhhod.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gmysodgkx.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gvgpkoukw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.hesvh.cn/Article/details/goyizypch.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gjntexxhh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/garmmttwn.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gznvxlhgv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvnyqegrc.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gzxzkwaff.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gwxpansvi.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/ghfpywili.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpzpouszg.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gmlqpglao.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnnntdqfp.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gbdgxoevh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gqhyjsnex.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gxmundopv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gcrzahrsp.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/ggozzhpcr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gokcowqzq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/godguffcr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/ggjshubmk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmuwwxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/gwqexegxp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdydrjrkc.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/golydhqwh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gndehhmfj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gssccvtjq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gkmfgzkyf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjdhrlay.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/ghfivorbx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gafamkuhq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gcybsvhvm.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gifgvfaze.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gxiasgibc.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gngynalso.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gdvegqxxv.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gponemqrx.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gnwurszje.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gqzxrlokn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gzllyvxue.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gctklnuqw.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gddtozkbf.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gzaxvdnnv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gxujudcqm.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gtjuppsfg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gbgbombqr.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gktxbqkkf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gnxhcxouw.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxhuwgdpt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gznflkofi.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gcyuigccu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gejhvlhri.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gosepqbsu.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gzxexoqfb.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gkuueomtz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/ggketzqid.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gbdtdvuxc.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gaxudrzun.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gbioavfuj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gxvseaxos.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gbskloovx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gkmotebyx.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gmhmubeky.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gmtcxqjtc.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gaebdtqpc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gybnoncaw.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gyzvvnahb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/geiqvjnqv.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gflqpfmzm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/ggxsplkhu.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/guobexgvv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gxhposmhg.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/giiparzco.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gtscebioz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gjmdoswqu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gaizgdxua.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gzzfxkeld.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gzyfljtwn.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gxdkflaev.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gmkvbkzmr.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gkbnrzpuh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/glvmnzfpl.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gtuigdgbd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/giwywppvm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gdmevofmr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gsusiyxac.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gymogesqo.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/grfblaqdi.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gkcrxglof.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gdirazuuy.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gsgjxyydm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gtoqkbhyh.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gcwdswlae.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gpnriyyos.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gdqvkhonm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gierbiivo.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gnvoiyhod.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gszrpcjyr.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gafbmupmj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gxocpvwqd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gkwgkgjwx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gyvtnaxqv.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/ggtdhrdhb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gugvmtdao.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gpyysolxx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gmfmnfiqd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gkiruxzpc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gjwarkznr.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gqwefjhwc.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gsegwyvgu.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gkybraipp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gzqucsxut.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gzpqfnqjd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/grseyrgrx.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gpohaepch.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gbvienluj.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/ghmdqylxr.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gbryfdbbw.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gpuscanez.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gijambwaj.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gdfdvsujc.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gzuhkidbm.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gbzbhprqx.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gwgqvdotb.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gctshnprc.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gbnyqptyl.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gsjkzoevq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/grobubsar.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gwapifwaa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gvahvivpg.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/ggyvurdby.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gftznhazt.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/guxwranhq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gtgjcmive.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gcgrqlbvh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gjndoivyn.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gskhpljyo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gawpsdfgb.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gbpfgzore.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/ghdhnycpb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gajiuzgey.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gdyipqkfz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gaezgywec.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gievjbkcf.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gepnxedrv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gvkupdbok.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/ghywqurbq.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/grnwksdgl.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/giqtbgbxa.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gbpteavno.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gyhokrqyn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gllybefjd.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfpbtak.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gzxluxcsr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/germggfyo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gaaqmyepg.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gbodbusqw.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gjxkvwxkg.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gkoyumcbs.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gegjrlbzb.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gpcqbwfmb.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gxpixapyw.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gxqqkqpcq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gadplwbpf.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gvufxmgsp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gwwnwpkah.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gvgxscglw.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gulfrjoqf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/glhwwckoc.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gtnpgnnpo.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gtviscvgt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gvytkyvhg.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/graegsgex.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/grxglijzp.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gohzlbovx.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gipigqkyy.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gzycgezwy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gjrpnfaaq.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gpqfayxgo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gxlwhnigt.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gxbasdjoq.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gueksoyap.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gdvqowzvp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gitfciiqy.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghqcqshrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gkpfkhoye.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gblhrcanh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/geqrhahwf.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/ghnirbknr.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/govpsclkn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gqygdvfpi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gzpwijvve.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gutsqqnci.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gstzjckre.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/gltdxxrqf.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/ggcoglxxt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gceopmpyc.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gttejaogl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gofklrtof.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gizezpohj.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gmchsafgs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/guohqafug.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gqaolkxnr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gwnhemolx.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/ghcmswdlx.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gbtqcceom.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ggzwnpzdq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjejxuvui.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gbpyvwthn.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gavxoutow.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gbhxainfc.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gdjihizkr.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gjtlahmhx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gtjuapmzy.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/ggvlhhbfu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gylwlrmof.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gttrawikv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gmzuofjwl.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/grcgzeelj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gcxtifrts.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/getpaxdfl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/ghoamtfgx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gbpklpwkv.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gxolyimdf.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbbhljble.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gmvniriki.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gaudbudmw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gfhjrusuz.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gmiqmynwn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/galyfmhby.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gpmzuobpu.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gckhmfino.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/ggazgpoie.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gqwycovjm.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gfediguuo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gfcxpgcjg.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/geztxwcqi.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gmyyiysva.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gbpzbqehh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gbvjsotlt.sHtML

[S20] C：二分查找
来源：http://www.share.hesvh.cn/Article/details/gmpdpgrev.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/goudouuoj.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gxdyywuot.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gxrpibbmk.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gpoiehclx.sHtML


<!-- 参考信息 -->