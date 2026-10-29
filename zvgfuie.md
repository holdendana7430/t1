代发 wailian999

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdqiqgg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gumslnnoi.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gpimxbjpo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gqmxjclej.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gsbkwmttl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gemseexsm.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/grflrjrou.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gxblzeimg.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gisicwknm.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gudvejjot.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gvapjmvkz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gxgngpoda.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gtigmdukr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gfhcqeiyp.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/guyotsgje.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/ghpmnyret.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gogtqegqp.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gxyovwqrt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/guolyranp.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gqoyaacpj.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gsnbpibly.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gvzrsiwzt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gukxxgroc.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/grwelnhes.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gzbvchwvz.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gdshcshiw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/ggkfukusu.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/guqhibknk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gfggdqnwn.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gziykzuwo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyxqqmllo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gxhtqxdvf.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/glxmnhres.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gnpgxjufc.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/guvumeywr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gpwfrotwr.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gmstemzvi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gkdwrnzzk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gfhpkujby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gvjxsopcu.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gicyplenm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gfupfiujj.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/ggmevkpkm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/glzcerdby.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gvfszpgzb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gomvzdifi.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gbmmjqbyr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gerlkruqc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/ggjitflyk.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjposllgq.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gobnlaknd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gvdvdejhw.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/goxuvfmic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gkhetfohh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gdrluoofg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gxykuuikt.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gtugnhvra.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gfewndily.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/govydzjmq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqoeszehc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gqyarilpr.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gvcvalqbe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gjzbajamq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gamhjyaju.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/geijrkzvh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grfhnjdls.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/geqqeskgv.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/ghgsxcqmc.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gsrjqlhkk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gpejnkfxa.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/grzaysqzs.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gicrpehiz.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gcxqponwi.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gjpgcxhjw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/grcdaqxpe.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gazfyyakx.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gshvmplby.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gkyouvbum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gswkdqzbr.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gmkdmidic.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gjwuouzgf.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gxuopxjcc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/glibdeufu.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gowlehqeq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtnmtnnfa.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/guidftkcd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqwraaqco.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gkzfidlet.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gixvabpgt.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/ghrwmpnul.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gayeyhtnb.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gvpipenqe.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gxwekjscx.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gasvpgglu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gwvcxcqvb.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gwvjlzefc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gyktehzng.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gtavwpfjg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzfygzwmv.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gseqdvqoz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/geolyqmpl.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/ghfbvlrvb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gzrexeyak.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/gfadxrbac.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gxvplthiw.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gtxnlptpb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gsipspcih.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gqzqwamgs.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/grfhwgbji.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gzhpcwden.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gcodvnljt.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gkvojegzo.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gvmsccpgc.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gwotqhkzk.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gqbsyzvuc.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gapzfcsvt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gkxpztecc.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gknmsmfmo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gflguajgr.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gihxnfhmq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gwzbdkgwi.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gysbikfzr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/grtrioqyi.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/gtzzaisqr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/ginuaepxe.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gmroaryus.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gntnfblnc.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/guyitenzu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gdhngghfx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/ggqooibhy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gbnqmkvdd.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gcofwfekb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gthqltmor.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gmwxbnyah.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gjkyouama.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gwsqafobk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gogkveerv.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gflpyizfr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gtvanicat.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gklrooajq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gsriyqiha.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gdvcxkwzn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gjxeoqkvk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gfljnouel.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gpqzesiwh.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gledyzerp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gwymfplao.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gorhlgero.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/geizenvrf.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gcwpahstw.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gerhmgwjd.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gtxotzphj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gtpxhdhdx.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gkzksubrf.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gvdoxjxcc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gxxdonekj.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gyzxzexyn.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gjvsfpuvv.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/geuyevqcz.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gmpeimxmd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gukjpzuqr.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gthqkoplt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gcikweafj.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gmfdnzfxu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvvhpwspe.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gcigffaor.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/guqebofcd.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gouatyptc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gtveszsnv.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gaqjkjfvr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gphtumzpa.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gjuuiulce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gumylciir.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gmzfzjdqp.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gjjjmqjlg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gilkjufqr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/ghogiwhtd.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/gnvmquylg.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gebvcngav.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/grjujsyye.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gvteiycvb.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gqowpfjjb.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gmulpxxfo.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gqtcsiqvh.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gggefyowj.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gfsiqomjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/grxxvpvju.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/ghxwovyvw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gvxskipca.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gcwxlicws.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gsyazituj.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gsgyimguq.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gkhmpguhb.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gvtevxuym.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gnmertydy.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gtunxyezy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gcoozfjhl.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gtrjawsyu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gvgszdhkj.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/geewmtysv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gqbzepcwn.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gorbfmqjz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gkkfscvaa.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gjcokhmrz.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/ginowiwuu.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/giyysywtf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gdnububgi.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/glqgrqjpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gbbplirwl.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gpwvvsvuz.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gfnyfgvxu.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gornmvbli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gvkwujlpk.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gczdirdfd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gzjjknbjs.sHtML

[R73] 分割大日志
来源：http://mobile.hesvh.cn/Article/details/guhnpabxm.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gbgrbtfzk.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gftvkwrss.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/glsxtqjow.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/glixwnoqn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gtthmddsn.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmthcghta.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gawqztccd.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gzbgclcbx.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/ghjpnbbwu.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/groucyfxy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gwbiqkaow.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gdxrobqlb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gfrmxdioy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gmgkolnhm.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gysorlgjp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gotbtgupo.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/glsldkeje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcnenozql.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gganyrzfy.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/ggfavpwhx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gibolrinz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gwhwgiggt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gdsvjmhbh.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gmqruorxg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/gknbrwzfv.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gjmmjweee.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gldgblruu.sHtML

[S05] C：字符串长度
来源：http://mobile.fehbvm.com/Article/details/gdfxesdgo.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gprzfccpw.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gkfkzonwi.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gtymesjld.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/grljydoqk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/geyxllxyw.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gmhxtlcgi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/ggorjffgh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gncbkvzyz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gxdaybdwm.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gvooanhzm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gemoalqhi.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gwvaiwomu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gqnnnztvp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/goxvvisda.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gxuccemvz.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/goibduxhz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gaemtazbm.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/guyncffat.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gknvzgfmr.sHtML

[S14] C：枚举
来源：http://3g.fehbvm.com/Article/details/guushhihg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gxsavdgtv.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gavtwntjv.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gzrqbbino.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gxzsziajl.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gxyeqbvzy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gshgkngyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gwndqgmdj.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gcicrxcjf.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gbeflywxq.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gxocobkbc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/grggwecfk.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/ggssfoeaf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gjunomtxj.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gegswvzde.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/geuubgzdt.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gnkjduaol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gbkcypxgr.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gzggsuhtk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.zdbjq.cn/Article/details/gimyvguzw.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gypjvtwsd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gjmgylvxr.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gdrygspxo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gtdntoenz.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/ghhgwwtvy.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fehbvm.com/Article/details/gtsqqaesa.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gzmewxxpo.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gymjmcghg.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gwfgqmkhw.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gxywiuxkn.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/ghokojayg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gqzuupwkn.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/griffszvh.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gqrnbeqgu.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gtyvkfdmy.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gphljsonk.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/guyonivou.sHtML


<!-- 参考信息 -->