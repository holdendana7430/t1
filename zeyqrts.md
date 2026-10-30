代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqriqzbt.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxsnprxf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjrqlwzl.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gqzcanwtd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxfclqom.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtijkemk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbgqtjjn.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkdzhsxn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqaqpsvw.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvddcmvvx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnfbziwgx.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gsysbhvpl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdickbfzk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gswtpvsnf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvdvqluj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxloqoce.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gjduivyer.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gumjchupa.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypwmjtik.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gaprxdcms.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gglrppmdf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/glguvopad.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdoywmtq.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gxumckvqc.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gtywgtcle.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gydeorzxd.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gcshlhauw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/ggsusmzmn.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/grorluvjg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gmqitvafz.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gfqtwjjzy.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdovotdlo.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ganzdiqyt.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaoxavkt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/geigbuqwf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosrckngb.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbcqkqbwj.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gtievkttd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnwqaiyt.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocmzyjgz.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvyjiqiog.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/goawgncmn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/ggsdsdlio.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gwknfnurj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkcrciym.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gcughuobp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyunccrzp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/guonpvank.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gatlzqshp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gomlmdwqm.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcprmljt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gumlhftbw.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gnydllxyc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gawswczms.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxogalfoi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptxqwuoz.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/guylxfups.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghihpxfyu.sHtML

[Q81] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/glpaejejs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/godvnlqfh.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdlllcia.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyceexvsx.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/grihkzjal.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmknmvaym.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/glklqxswh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyoukhgf.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytcoeklu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqzctwu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddixljgk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gxyohtpnz.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwxocywb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gnnuhfvjy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuyqjluc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxlyvief.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzswogwcr.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpeirykpb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gaqaczmbp.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gklnubqit.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvhcaxob.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifabyxuf.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnbzaoqz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtehuqtpc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcbyymlz.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gbvrosjtw.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwqsslxz.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrecnaoq.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtxlulqa.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/giyfyzqkq.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gymakysen.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwbzuttcj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyhfiiwv.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyggckpi.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjlfugcx.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzppjqisg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnjlmizm.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkkxkdja.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmcdooei.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gehobdrrs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/guofrrwjb.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkziwhblg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gwankrwqv.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwfxxjadx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxbjslsxb.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdwfmhtdg.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/ggtjzkznm.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grelzwjpo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/giywkvhwc.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guicfrelb.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/ghxnlwqtm.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwngkedru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfvcvvaex.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/ghonfyuqs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjokcihzc.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/ghlcdngmp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkefrpwmq.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyfcmksz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gegzoqpqi.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/galbqjlkd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghjnvfqcv.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/grwezixtp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzkkigs.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gincyjitc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gptjwhexo.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzjqqkidz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gribotmvt.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gnnmexqbe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqxfftkkv.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/guthhlvdg.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/goyiifooc.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/ghuddxfpy.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/giqbzrvph.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grqrddkdv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gdzjtbklp.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/ghwbdwmcv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaojehzgo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsnycysc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrqxyima.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/glbmohcvi.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gajvdbzoo.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieoajakn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwtoniti.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gdkvgeahf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsalktsr.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxowcbbm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfeoovoiw.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gyxnxnoiq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncfjjbru.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggdloqqzc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjmonhveg.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gamvipsfv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gystchoyh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/goompbloz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvymnbfz.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gisqvljez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzhjvgxap.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhcuijaq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyrglxsm.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gnklvpibf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/grdttsywz.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitnwnmtj.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdwpehlr.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmcnhuro.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbsrwhus.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gojfhzvfo.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gduoimxan.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gtjzuigvr.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmvbnqbl.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyculyvn.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gbhllvsic.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gxaxjnqaz.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glgtkiotv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzmempvj.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gdimizewo.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnxxkjfn.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gixnmdyip.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekquhmbw.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gexahabub.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/grhnbafma.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuluxflz.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvlcrrxm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvakibaj.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gjovrfgyt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glxeoiqby.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gxenicxad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gsujbbppq.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkeuoddo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnbszxqrd.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyzfczge.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gtjhkzqos.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwervtnvn.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlljmrrm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gvtdgmfba.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gjejnukio.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gahlhtecb.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcohfrss.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gthnaypnv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwvflgvd.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxvbkpcl.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gyqquyixq.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gvioizayw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesgqztzg.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gcyejtlho.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gkpcfqhlx.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgwqvjat.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gazumxhpp.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtykjbwgu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gkedzrgjr.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcmvibks.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnobgxcdm.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkubmfqd.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoadhtfb.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsjgxzfh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gytjkqxet.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gutkbzpdp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqapurh.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/geybuiljs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gogdgajrp.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gjtcevdtr.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gximbcswx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gqutqqlsd.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwiofvwd.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtkpmkxv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/geamovrrp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemlvcjt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/geppziaoa.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfxjyxrn.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gdgtsmjgt.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gljgoddwv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknvbxhph.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gegkcznxz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gamwjpjcr.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuwnmuko.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gddurtlbb.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxxozqru.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gearwqdpu.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmkqxeymg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrobcwhb.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbodtzvrn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gktfcjvqu.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpineyays.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrbdvofr.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/grhucjnaa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gafrtsaxf.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gpdnuxwky.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/greeuwuqk.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gerqzoykk.sHtML

time ./run.sh
来源：http://m.share.fanxiaobao.xyz/Article/details/gaslzrwdq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaidqucqv.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/goeusjfan.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gszupuull.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfsvmltj.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgjzhwpq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmywcrdtv.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/glctvmckp.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrfcolcc.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gblfltvlc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gztsgtzbd.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gkngjnzsw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gtberzujy.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghndwihcl.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gczcujpjk.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/geobnllxc.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gczpcnwht.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvvsuslq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiilehab.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvbeqwdd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxawqwmp.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gpkgsdrxb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gisaivooj.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gjwlepkmv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gufmkdwjq.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrxbipvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gowkbfdzk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaqtgiex.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/goiicrfqg.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/guzkwdovt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzsdqajyv.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwlqkmui.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gvrldpuxb.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfppuqbhi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzekmhmgk.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpldzjtbt.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvzpzkxof.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/ggihwwicu.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/goypnhkja.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnekqlwf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryuyivjm.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/glnkzjjud.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/gaawpxlbn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnaxtqzd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtwhtbjc.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvactnql.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwcsttnb.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/glrhhyase.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjjoyjp.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gujfclwdd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gywookbxm.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gdhtyxbcu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gocqpsfac.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golzatvkj.sHtML


<!-- 参考信息 -->