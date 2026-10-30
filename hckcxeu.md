代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/geknvuhtr.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhnypplv.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggprzrsua.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gpigbeall.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjvtuezx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzrxjyqz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gpfbhgntc.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoqahzhv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqiaiuqt.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gacpclvkp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvngqxpvt.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbhqrzox.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gajorsijr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfbsytzc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbsnllxe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzvuhwlai.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gebxushey.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpokatmad.sHtML

[Q62] 分组占比
来源：http://wap.fanxiaobao.xyz/Article/details/gryhycwnk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gactftayu.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/glfepbidr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtwvgpuj.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghasgzmde.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/giuuaersv.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gycmtzoex.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtkrouzs.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtuuawhgh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwfmmdcz.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/golixkvxy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gvsxxxnvn.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gdltbzaha.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gplkzvqbc.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gybgswjcu.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gjdxxuozd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/ghpqpyiif.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gczykjwpj.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmxsbvjz.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/gzcxancbf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgvxluiu.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/guyqsteto.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbjhbpbm.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrxheeir.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gyshywjhz.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnwoiuxr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/grooykctq.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gepskmzeq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlnkanvi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/glpquetwu.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gmscrslhk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqsekmqs.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhhiemdm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyxmlzzx.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwzhqjoa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gjucjnniw.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/gnijjzqwb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhamqpqi.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzppgzygz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmucygmof.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grezjiwml.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxziodj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmnqiqoe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdmmaqjrw.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwbikstdv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnykmaaix.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneudumoo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmbxjbaf.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gagmgaypi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gyzrsgscu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyangqyxx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/goujdwawi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtetpfmjx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gdfhawgfg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gebchofou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmvfkeml.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gksyspekb.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gzpuibngd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeotvmcm.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/glvwxrcag.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtsxkhid.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorjrferh.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gndzqtuxv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gymktjjkg.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gggsrgkmx.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gmesxhkah.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gqjsvuaiq.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gnpxwqbit.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gknxlgapm.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpnuwbhvb.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gkulmpqrc.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gejuzcitl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqitnprgy.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhbbqyyc.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/glgslkfco.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcwmppize.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghowfsolr.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/geevygnko.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gffvoytyn.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/glyfsmyql.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmlerhyb.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfsgelzr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvjdoptn.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gfotpmmgu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwckinfer.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvzjckhs.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gzhugokcw.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhiglroc.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/grtkmeqgw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gprdgwsls.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuucsodo.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gztkzvuar.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxmsgcom.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gesaxumim.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbcthtde.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gtlggeeuo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaboaykf.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcwqbxdto.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtarojwwl.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbnbwudn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grfghtmnt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfwywqvn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmguynky.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gbtvwehul.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwpeztvqb.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gekhyrfpi.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtlyelim.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiilskfo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjvfwofvz.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkcmumdg.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvkrrxkh.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gtgsfaret.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqabqjox.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmsrtvoxe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gvmvjgqke.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gygkiusjb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtjixhojo.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gtmypxvsx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrclonek.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfetsooh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gziiicdqg.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnhgarbf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gebinkrxq.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gznxblfbh.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/golediznd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrdlzegd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlgthkry.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gpnddtnwi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gecglxzds.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxjbzydf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfhhacwgp.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gyzgbfuek.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsdiaapju.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhkdnjki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gpfzkijtc.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgrtxizz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/ggsxjdwud.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaxbrdox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gmnmvetkp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gylukwxlz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/grwdhollz.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgrabbtn.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/groehqbsk.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gedgnakpi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/glqhrpuxx.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gvcfhznxf.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyssaqix.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gwihcilko.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkntdlthy.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpnvzjvx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglfsvcwp.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrvvmivr.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwajgucgn.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfodlssjp.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvzqthjot.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvojewyhj.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gsngdysve.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gnbwolpsd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gikozeskd.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gukxlcjwr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gdlcebcid.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghetyzyew.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gscbujahm.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/grwiuxbuf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwsxumaum.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadsabnep.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpsfsloz.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gpvwmiuyp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhlojhxi.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbldawlj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/guifyzrff.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gquliwwoh.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxuiekbs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gygbfqqqm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gheginweb.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/glmbdzvdc.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ggdhwiwnh.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gmrevevpg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsttppncc.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/goxmfbomc.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/guthimtgr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxnilptv.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gxcwqtoqc.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgopsyje.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/glvszzbjc.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gangmwaig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzwtoujx.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gklnrnqwn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gippfigff.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gqigjnaec.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpvmdbse.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxddulta.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gvrgdgoeo.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gshbffgfh.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlywcncx.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gfzmcbzen.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxegjnts.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwpkzxrw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gedmwtylh.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/glaftgcvo.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbipfpjmd.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gjdygjpnl.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsdjjezd.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/giwblwign.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grzolhsnl.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gshibziev.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnhizggm.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkeseslt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gglprkuvp.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gdprmbohj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gvjhcqnza.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gpreyykqr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gzuhyysoc.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlwuxrsa.sHtML

split -l 1000 big.log part_
来源：http://blog.fanxiaobao.xyz/Article/details/gmgsbtbsz.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbnpvztx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gulbaiwlp.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxejoshec.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gpicskkoi.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmrvjiqz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gipzbnwzd.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxpoehxg.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gcqxbvlls.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpkmhvzf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjojbdeo.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gixxjhelg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwwacxgp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gslllmxup.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvgjbajo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdxbvztgt.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmspemtti.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gslkzloce.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gcdgjdwfo.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvcxexue.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gynilciwt.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gmstqqfwi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gpojxycsv.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnayvhvqk.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlguyhyi.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gpqrmaqzf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gteqhoflv.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvtafuvy.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gztxhlvzs.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcgepjeb.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gejatjmnh.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gcarpwedq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvjvrmlu.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gmzugeent.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmxeybka.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbvfgvkn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/geimcusoz.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gbrnogjev.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/guqnjloqm.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gntpknqbw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gllacagka.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/grjcupxuj.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gewjvzmyi.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gprycfeaw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdlhlso.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbbacgfc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqglbbcvv.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdgfskxdn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gjwhynhee.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpniohrvf.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gfjugmyua.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gnvvmyebi.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gixgntsen.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/geyzkmwno.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfptovygu.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsmtwojxi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnsxzprk.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/grjsxhmqq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyspqylqe.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxoyovor.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdednktvv.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gtamuilki.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuzgotco.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/ghqtdshle.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gogjoaxps.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gljosqhww.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gxyjepoby.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gkulyznkk.sHtML


<!-- 参考信息 -->