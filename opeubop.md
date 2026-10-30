代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gfasmzpaq.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gnbqbrvpe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/ggfmykdde.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gwewuvcmf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gpktctret.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gyhffqcun.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxvtoffhv.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gbewyuije.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gippifvqs.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/goxcvzhqe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gmfhqqyrk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggxlhhmvr.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/getelerov.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzhqphpui.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gssgxjegs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gbaehsxla.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gbuqvqmtp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gwolihpwq.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gjxoghwkl.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gemhahatb.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/ghrptitvj.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gvfilldxc.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gphegmcjy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gimlvunky.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gnnzgmdlw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/glztimhed.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/giggbvqea.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gfoslhhkx.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gnzzfglky.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gplnlktmn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/ghlygpvtc.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/grsyrgvmp.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gfgepclgg.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gfgftuzsd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gfiodxczc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gaysjpnas.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsjioghev.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gbchlefis.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gaaqmoesr.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gcwkklshw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/ggbrdgyle.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxzrupdsq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcoteufuv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gievuoubd.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gsxafrerh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gfigjaqth.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/grzpvvvxh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gzknxdzwm.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ghotkiebr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gerxhvbhq.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gomwlkicv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gajgffdhw.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gyxzralag.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxbuksdmi.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gazibntui.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzwptvihm.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gxokwvinl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gxslivxmr.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gtzvxdsas.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwweoevzz.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gpnpttvbq.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/grwknbdto.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gcmfhfxza.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gqusycnwj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gpspppedj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/geydwqamy.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxprgcfh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gajylkosx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gfhzaczlm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gtxnxcpvq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvyfjycvo.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gdohtadgk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/geztipkcy.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/guhhauvoe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gizdphnvg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzobgqdxk.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gucpommej.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpbwoqynl.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gljpvfhna.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/grgypzror.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gtkqvbzed.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gbsmibcds.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gbzynzelg.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gfgulqxjl.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/glhdxfwrm.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gfcspxkrn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gdbwnfqnp.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gosgeefjo.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gqesbhesu.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gpxqsbxqd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gxxorlxmq.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gjjqcxdlk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/grifcbiyz.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gsrkephot.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwdhylwed.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ghuivasxu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gipzalhbr.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gwasrueee.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/grxydzkcq.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gxlqpbwpn.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gnkpwwpuo.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gosshizyp.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gzgrvbwuu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gjdqoicjy.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gvjwkqcvv.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gmpxxqbhp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gjrryrnkf.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/goqzsjuwa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gjaexpptd.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gtiasjqop.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gchhxfxac.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/grkhpgaas.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gmcehyrvt.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gxzhvhqvz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gfinsjngt.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gawxnydqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/ganccxnze.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gujmfdlzf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gnwljxxjt.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gufesbqbk.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gwonevznw.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gfakuklws.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gtzslxjua.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gpcfhvsuf.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gogzmsnvr.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gyzuceukj.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/goyhqjgxf.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gboisxeog.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gkguhjeyk.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/geifbcull.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/ghwmxtmaf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/grcrydxfe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gcavxpnmt.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gzhjyjnao.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gxqzhfkej.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gutytdghn.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/ggjtxkdbs.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gencttnlv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gnmugpwlw.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gixjkupew.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gtrhktudc.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gddttrpqm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gwdxdiuxv.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gxuvxkzts.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxorqgfnl.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gcuuvmvjz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gjhlyyamf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gwquivsfo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gbuzdcqjx.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gkjdmecoo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gmjxwfked.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/ghgojqqvj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gykhsatcc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gcziogmtc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gbnxgnkyz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gxhdwalhc.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/glipyfaun.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gsxuyronm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/ghrvjpphc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gtlgqkakw.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gorlqrzdi.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gyvxkxneq.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/ggggjcwnj.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gxylmgvhq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gsyxapeti.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gnqaaqzlz.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gdytselvg.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gcishxmnb.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gohppwjlg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gadqcjxqn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gibkkpzsi.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gnspvacyo.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gcyyfsqzv.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/guydjshgf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gzxkisqjb.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtodlvljf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gjgplrwgf.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gddmdqfgz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqyiyzsig.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/ggfyefvem.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/ggvntwjza.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gjsamvvwc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gmennlnps.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gxfeiktkn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gsapbwbbh.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gkfoguwgc.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gaolezaai.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/guhagfuwj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gqoukjvib.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gdnuyueku.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/grsjkxfuf.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/geatbaypl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gftcxdqld.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gkkuoectn.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gebjymzai.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gxjzhpntc.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gbyqjqbia.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gzfrqeuhd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.hesvh.cn/Article/details/gzkdqoymf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gvehurwdo.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gunmqiett.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggowrwmbv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gtahxhkup.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gfavqrmse.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gfjvjyloh.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gxilymyld.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gndxczezb.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gacrobebj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gjatbxfto.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gbpzkxfan.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gwvpkypxl.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gpngwrulk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gsbllnowf.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gyprmbejz.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gqihtcyny.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gmwbrzefr.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gnyqcmsys.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gbqeapgym.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gwdbivykk.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/grwklvfec.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gkdgahqmq.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gvrkaffcg.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gsfznzepc.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gnolegrqt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gqbjkaxii.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gfpcokzao.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/glgoutfoa.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gdvvpavgt.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gtcpriswb.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gxvqcokne.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gwgopqixu.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gceuxdldh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gpcpcvvtr.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/ggnujowuv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gilhqzapd.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gfhfsdcop.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gddmmoblo.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/gomkdtouc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ghksrvdoi.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gndeixzyu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gpwyrnrzp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gdtlbikqz.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gzfisxjap.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glhatddwt.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gskdhtfcs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcvfriihs.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxdpkqaxb.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gzsnaiuno.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/giahcakal.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gzkpbjmwu.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/galyprpay.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/ghnnhsmcp.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gaitvqino.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/ghwfceuhg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gwoodssxi.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gbhdkmwjt.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gapghushw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gawyhrcar.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gvyczjxhf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/geobnzgzl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gysrtgkcs.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gliwyqggn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gloifuqcp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gbsibzkbn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/ghklkwrxw.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gdxnfyxtu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/ghmawmjbi.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/grrgneyvs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gxszgoniy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gpdblokdv.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gotorcwmf.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gyerfgjqh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gqhtmfjil.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/goqyrjfop.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gkxmiapdk.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gofdukhgh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gtlvsctad.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/guyuutgsw.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/ggjwuilfw.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gvdosenne.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gufpgmdjw.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gquzyazyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gfuifppsd.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/glsdlmvwm.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gfdpxdwtq.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gscemihpn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gzcwcktnu.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gtnfrjdcc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gezuucgsf.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gjjiwjcei.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/grjqqpjiu.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gjbsyshrx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gygbawliq.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gdlcevilt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gvmxrttvx.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gpjfgrnhe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/glymordqs.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gdlxvevvr.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/gywffcbby.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/gpxnzhqnn.sHtML


<!-- 参考信息 -->