代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxuvzkoa.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gaglwwrxe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gybziqrtk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gzndsnyjz.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzityznuo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjhsycdv.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnujnopa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gbajikyjp.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gvieufwot.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkftnclu.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gelnalimy.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gebafvyvv.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghspmgfww.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gzbiwxkaw.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtjhroqh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/goxbkemsz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gygzfnidi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gqrgqgkyu.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/ggeeclvrq.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gsdjuywex.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtbaohdzh.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubjyybhz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbjfgcsr.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gkaibasto.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gaqjcdpjq.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyypnvgpo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/ggefhkhzj.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gyrfbnadp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grriengcd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozubeobb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gulqcqpdg.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gxscjhhex.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gloorhguc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyahwhsy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjhrnkbf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/giyqnimzn.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtkdpbmc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvbywlgo.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkbbeloq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gulszvgft.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqahhycam.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gkunmwzqd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzfilfis.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpioivsu.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gelupibpz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkleyaow.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giwjqxgxz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glqrjekrl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjmpvtgv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjbzptxs.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpidjxbom.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/guibwdzoy.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gahcqvphq.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkqzhkhat.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gevjbguyb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvptlxcch.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gogonyxjj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkqqlgok.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbvqtayhy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxhvorrd.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/goyrzcexn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/ghnigoyhl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gesagtdfz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmospuac.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/goqxommmq.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtglwcyk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gcqpshxma.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkwthvwbx.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gpevkoeyo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/giwoeibfr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gsujufhgn.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmswjvvs.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugjfjlfz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/girrumrbs.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgxrfvjv.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqmweca.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/ggypzkcbb.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzcwkdrsn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gnvmurpzi.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gqzxvoyaq.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjxnpixk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnilrcohy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/garzjlpzy.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzjpzywya.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gngdhfzie.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gdvdfmpte.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gdryfrptq.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gitjzqmuu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfdvmwry.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsdtyrhk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/geskpbkkk.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdfziftc.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gtpnxwtmg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuqjxxmq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfqfcpej.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/guznuqvsa.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gyegdbmir.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexdesuku.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/giwaszulj.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaxaagij.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnfspirch.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gnkgbqbyn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmvaiitva.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gggatjncd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnhmaonx.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmlxfivh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzyulbol.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gfikbiwpd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyokwjwwi.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/grvkwmcss.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtkkywea.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gaccjlvke.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghpdugovv.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gyhldnmhe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkpkqcit.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/geetuedqe.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnupdbnoe.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvatpzrtz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfckxclc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgwwqmtl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gddikgkuf.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjzwwxac.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuxxjrqf.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtwgtfjk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzndvgomn.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gseggnhuh.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gbetpcjlr.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gvvcrujnn.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpqejofl.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gheptvqug.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdemlgro.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/giddpxmlm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gjrggkptj.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjsdntup.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/grzhsqnaq.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwwaeurrs.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glmpsuyxc.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gzywbftov.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gasmdehuq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gcrwryrfs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/glfrgvfuu.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gyvlwpcxn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbuhasmg.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/glvubvkne.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/grqprwdyd.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gpltclhih.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhffjzfu.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzgxrbzuk.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/geuomhlhs.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gcswbrkvh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gitjymplt.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/govgkukth.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfycxenuk.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gpbefmnqd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpmxcnrs.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gbylpeuxp.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcltzpcdc.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gekuykoch.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonvyduei.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsealfqbl.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gfjzjojjy.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/garesdqvt.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gruucfcqd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gyqosijwv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvswwloy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gosrpevyu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gedelhrip.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdlplvaso.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gadxdexbz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtayyywlb.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtrcrlte.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/geqqgsdjs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/geckdevxg.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpegprata.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gooofkqny.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbndvwix.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gmehspkjc.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gslzbcxyq.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goqasqvfx.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gyzyefjye.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqojfpckq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsyrblufu.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsjgmqcl.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/geelvmskh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxlrvymx.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gdacklxut.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gigvvzhob.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuxvxtrw.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/glnguekwt.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gstcuqohi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gprcocssm.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/guuwvwquq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvujvxbr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gojfzsksf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gojxoxpfp.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/ggtwytbtp.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gsdbjcsuz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gczjuksvm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gcrqnlret.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gldbfuzsx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfpmrxhr.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gsmejlfek.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryirzsed.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gskyjuyby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fanxiaobao.xyz/Article/details/gdtkeygqe.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwryzraed.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsvkqvkl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvezwyhzu.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpjwehbi.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gkjzjlbft.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gchwwcxtv.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznubukmy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikrnefba.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvzgdgc.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvcsbrir.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofmohepz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/guvmtrvgb.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gwqskyazm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbzwgebt.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaglxdzf.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gnpgzcynp.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwbabqow.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gloeazjww.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghowwyoqh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaszrecak.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guyxpwkob.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfznqmdk.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gbanromgb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxkqcnqb.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoinlqlt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmiikqhc.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/grnsjbmry.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweyzcgtm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpdghrto.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqemoum.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gepshdwhz.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gsyoezahn.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grqurwoox.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhierspe.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmneuvtnw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtydyatb.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokdkjgmg.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gikeapzch.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzvhtrjl.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/ghbsxjlxd.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrrrznl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuiwnjqg.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzjohobmz.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/glpinmljf.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkedjusy.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gzvkiwywk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gzuvoeysk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiwjyrwc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gtnohodyn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gwhgymgks.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gwzqlejdh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gnkmprjzm.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsypxmnxb.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpzawgbw.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeutnrks.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbazvxq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxewvmox.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gstgeafbf.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqtiqffuz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getrvlofh.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gsupfgshs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvdateis.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzdoxrm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godddztll.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gupjtqkwj.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrpwjucr.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gwtthhiet.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gdrenkium.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqiabzcw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/guihcglns.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaczkhaw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwdtavon.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyvzikujm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gctubnnod.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gmujbmncy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwsrdici.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gultugrte.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/glpjztvbl.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmacukhn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gllnmbuwt.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpedlxgdb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gwahykxth.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvfxzpzc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjvulcfh.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyyasnut.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gbmpfhmrj.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxjjsraf.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/groqnswac.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gigpyrwha.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gefyuzvor.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcndnvdzu.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtrvzazs.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goraebnkv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/ghojbdhld.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gqlszmvfi.sHtML


<!-- 参考信息 -->