代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gndnznpyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gobkzmaoz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gklyrqkrb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/goshtkmmh.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gokakdsaj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/giqwfnthy.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gkcgssuhf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gsvnjgrob.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gjymidvqz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gtjxjsscr.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gqxckjxum.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gjabodjez.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/grmaxwydm.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/guiwoxale.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gqwakchgc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gmerzfsxs.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/grpmckjje.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gkegxlexx.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gpjrvzoau.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/ggjyjydfk.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gwoumzlxc.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gwyjyxohx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/guluaepau.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gontgulyn.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gunakqdnb.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gnqehywtz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/ghdmsbzag.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gzprbvkiz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gntufyjmi.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gzcttzaez.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/ggawssevk.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gniokyxau.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gegxtbpor.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gofdmprml.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwwahmilb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/galwslnhf.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/grrygtgcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gqqebzqwe.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gktsumznw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gzuubjgcu.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gixrxgbum.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/ggctyhjit.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gpcnjovmx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gqlzawlia.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/glunensud.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcapfytpg.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gkeazmyqe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghwxxzhhg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gbrxhefzs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkcmmxymu.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/grgllqrxh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxgelbnwv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gaeogvrjx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gmppprmvd.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gdvijspib.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/gofoznciu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gpsqavmcp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gwlcgrqov.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/guanyhykb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gfqikjuey.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gducmdnbk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gpuxnpric.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gjxgtvttb.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gttxcyvbu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gmaafobzs.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gfgofbnfa.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gyqukdqou.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grtqqhtse.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gwxbiggpz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gidqykjxi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gpayhpndv.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gnzlvrzgb.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/grhyuiorx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gmwcdgyqp.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gzfeiiufv.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gbvyfqlsr.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gjnnzazci.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/ggcltlbcy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gvlabcnlv.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gkaoylknk.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gpqgpqfdc.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/ggrbgdzjq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gcujzzcsj.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gehcxewsk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gypofnqjz.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gtvbdjgwa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gtyhmkglo.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gzdlnpnne.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gefptjzdf.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gvzpbxttc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/ggdwbdoer.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gdgjdjdwb.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gyscuarwc.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gwrhiiiya.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gadleaznr.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gxaystdea.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gupqacrxw.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gnobbdsua.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/ghepsdqhv.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gxdrcqklm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gbngtwcqn.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gcxeyvsav.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gojfupznv.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gszvrhfdz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/guarvlemv.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gjyynmqgl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gzmdbwiej.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gtnvqtnyv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gxykdkvxo.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/grigavjxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gyqfzaqpq.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gzleoxbjn.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gdoduqexw.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gbrxbjxqj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gujbmtvlh.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbqureevo.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gcfqyplbw.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gnlgkhzmm.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gakjayjsy.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/grchiyjxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gctikjybs.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/giofrczsn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gshtaeiqb.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gwbkiigia.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/grnfgvkzi.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gvlnslkef.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/goplndjpl.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gwbverwzm.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gplzkyvvm.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/giuhyxoqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/glhpzkfva.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gtbfpyipo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/ghciyrbdy.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/glxgpvjif.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gsabgecew.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gsllyfzwn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goeyyabqy.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gvdckbkcy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gagxrfxvn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gtxmuohth.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gatcqdkpc.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gpluzjjeh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gixzoicfz.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/gtxebudql.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gmkzcaith.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gzoqvpeuw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/giemmjknt.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gdqpvzbmj.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gugqylcrk.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gqqfleney.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gqxzeushu.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gygivqfkk.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gukaoixql.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/goabyzwxj.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gamkgcpwh.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gqgsdcxqp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gopbedsqr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/geemgnfpo.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjzfrhdfj.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gzwufaqyo.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/glucgabzv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/ggdeokkva.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gjefknhqr.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gnivsmqys.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gjvxajnzm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gtfnmmkum.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gxscguqqh.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/ggcvrjszj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gzsusplty.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gaeceigtc.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gqlhpjkyu.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gfjtzwvxk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gdrbarvnk.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gcjfcytrm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gcgfztnco.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/glguxinxh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/ggagofgdx.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gvxwtxrbf.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gweadjvzx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gbgptbinf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gtkklhluc.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gemodawhf.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/ggdqnwdjg.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gqtnlaesg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/goqmkzequ.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/ggabhhnkj.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/glofgcjwu.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gzisosjgm.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gcsibamhg.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gypxywzyx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/giajeqowe.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/girrzaihk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gaajwskky.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gqbvtfruc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/glpyawsbf.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gwjvadkbp.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/ggprmtlki.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gusafrybr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gykdytrrg.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gwonnmgdo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gmtavfsxa.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpcahmboe.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/ghyorztlk.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/guudeaduq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gnvuracwz.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gvqqjocst.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gazhxhepo.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/ggmbkefdo.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/guhvpczyl.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/giwyrxmkl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/geprhlxxc.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gwuruaqpq.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gxmvocwco.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/genhglmet.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/giyvbcucy.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gucfypwdz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ghgfetedw.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gwtgxcqtu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gpnhwfchc.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gkjwjoyoz.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/guphtofgt.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/ggfwryyqs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gflgztruc.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gdrbrizad.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gxqdxowia.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gowkogdaz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gxfkbxuug.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gqhsydgcd.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gvnvxzmkf.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gmxfwmedx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gpxmjpbvo.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gzsuijwyy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gsxjcrmvq.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/glkyzptbu.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gqnyoehwg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvddvzbdo.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/grtiestie.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwusqtmez.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gaemfacim.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gksqfcqmx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gbuboryfs.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gsjjhppam.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gpmfyezku.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/grbxxjxia.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gicnxhgen.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gsnhpanhr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gwftaynpb.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gjoaawbgd.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gscatykgg.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gwjciikzl.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gztttweau.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gebyvtced.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gshuusvjx.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gdufmbmtl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gskqnfzsh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gnllmjsdx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gvabcsfff.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gjylbpany.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/glnstymhp.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gkjllqhbs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gfoolxhml.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gylznwyzp.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gknhrweun.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gvvsdmwmn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzfmzkk.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gunzpsvos.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gtvygedhw.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gzcroiref.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gpwqdaohf.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/ghafmfslz.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gfabmfbcz.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gnpqhxdmt.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gdlarctwz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/grvjsjepp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/grlmzbxvy.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gavtaowzn.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gqfxhmfqh.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/ggovpddqh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gbuapvmrb.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gspsesaqv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gtvidpjcg.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gvpmhargv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gfyuowjea.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gvgcdbnsi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/geqppibbj.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gmgrzocok.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/glviiamjg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gikqcskth.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/grhoauzcc.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gqftdhvre.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gtbwyqhht.sHtML

[S26] C：内存清零
来源：http://wap.fehbvm.com/Article/details/gmiwdzuso.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gneiypoln.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gydmqcbga.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ghysxzwah.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gafzjnhwj.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gfwuxilti.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/grfdoypzq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gdecmsnjn.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gmmivvrqe.sHtML


<!-- 参考信息 -->