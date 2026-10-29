代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwjqkjbet.sHtML

[Q58] 累计求和
来源：http://wap.zdbjq.cn/Article/details/gsalhvrvu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gumchdybk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gfppjsjmp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcjhmwcvb.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gbxstntry.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gxzfsaxlf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gxixesdcr.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gypgxbrqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqbkkqora.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhcwjhm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gdnmqdfxh.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gzujotmbw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gapiewlmg.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gstpmlzhp.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gyitqcbmm.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gbazuhhpp.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gmalycfbr.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gbuxminde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gonblffio.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gfkexsnis.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gxvombiuf.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gefrgteiw.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gfhzxhkmp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gffkpgymi.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gelengupo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gtrztjmdp.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gbdiutlil.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqgldnl.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gxotblrub.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gqyhsghln.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gizpwsdes.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/grjwznkqr.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gbqwlvrae.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gxxdewrft.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gjhgqqpcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gplopastc.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gerxjeexg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gfoweuycp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gtrulhytw.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gzvsghorw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gicjbygil.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gixqzrwej.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gkkczsfcg.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gswjaosry.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gqcbmnbmd.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/ggpyrcyfs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/grlptlewb.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gdyhtzlcp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcxmeyirc.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/grzyojiny.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gtmbshvca.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gipoqnsyn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gidbjtiwp.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gejscwgxw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmokhygqf.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/glapkqmvq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmuzuaygc.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gyilkslic.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/grynrztme.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gdxfblkic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gptlxserb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gcnteponr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gecqzwukz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gupmgapsr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gnjeszlbm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gjwnjyywm.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/glwmiovqg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gcglptdhm.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gpkdbjusx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gzmrjqgun.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gotrfzpdx.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gkahipnxh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggkaighvq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gjatowweg.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gihnaubuj.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gdndmlxkd.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gwpuqjdif.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gmxwailyk.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqaieqynj.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gqqbenzhw.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/glldfptcq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gbryrtlin.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gaeylvktw.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gqvnhwfsh.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gipzimbfa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/grbivrodz.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/glluyesdg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gdkdajmfz.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gsmwtlykp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gqgrtspbg.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/govovsumt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gfdcgblpm.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gcfwrfmhx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gfznljxuf.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gggtmwizq.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/ggjzpyegh.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gqhqqahqa.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gdkawumtt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/ghasodqvx.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gmlgprjda.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gltltseru.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/gbfgeiudt.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcnarab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gxkwgudcq.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/glgbpadcs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gxavtwnax.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gwvkjdojr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gpnnhwbkn.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gwtapgzee.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gvybbreyc.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gixgckkam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/glfwxltrk.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gcctjdpuc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gmpobqxkc.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gvgowvbns.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gxgjtswyj.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gnehdrarr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/ggvfiprvq.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gxtxfckqm.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gosmpysum.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/grbnslkfi.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gnwmnvnmh.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gnooydzwy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/guzfuleih.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/guwxlfofn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gicnvyiyg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gqubngoad.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gskhlyfms.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gmqdftymk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gjxtubacl.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gaxulmaov.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gpusithyd.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gbpkmxlkn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gjmvpfnyo.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/grrdyoupx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gjfhyrbqz.sHtML

[R30] 函数返回状态码
来源：http://www.share.zdbjq.cn/Article/details/guldolijt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/grghrgxaz.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gucsyrjnk.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gpmxcunqb.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/glgxicwlt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gcvxkepjd.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gdgrjrsgt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gxaunzzab.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gpgmzsrrk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gpjyvmhuv.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gewiihgmt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gwiqjpidz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/guxtuemhj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/ghogapfur.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gthnnrxwl.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gjbcznaqk.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/ggcxktlat.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gfvsnptod.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gtnmocens.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/goetskvdh.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gvwtfqwix.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gdmwrjhhu.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gwuhptxoy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/ggldhpmiu.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gnfyohzwg.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gnxxkhmaw.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gxmgsphmu.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gvuzcoplr.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gpdmuupec.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gwwfzohie.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gnjqvvowt.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gplejdglt.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gondpkcbm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gmgfuxvhi.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gcaqbqzdh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gtfjhstny.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gbytfajtc.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gqfmsjxzd.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gndqjqpxb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gkqtcsigp.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gvfhstmyw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gfvfuhnku.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gelcgmwks.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gzkvacqgv.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gwutdkrka.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gjkvblsjn.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gfjceasna.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gxgaecfgk.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gnmkujhdo.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gkozyzwyr.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gyazstuxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gwqhbveyx.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/grboksava.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gyjfnhtgv.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/goeimmnxy.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gepnwijyb.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gmdiubtxx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/glyfjpopk.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gzzabhxrn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gcrimxuvy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gbyniicto.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gkcyshnxo.sHtML

[R61] 磁盘占用
来源：http://3g.fehbvm.com/Article/details/gkqxoymxp.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gxdodrujt.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gxtnaxkrm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gpfeixauw.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gzjerwuks.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gyhcxrfyl.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gbbtgjzvk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gzyvmiuwx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gzpaijjdf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gexnwrrul.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/grhzjspwr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gxvbonpwd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/gcucseggh.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gbtladjaq.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/geasraicb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkwmidawq.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/grrvfserk.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gflkirwtp.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gkyusbtve.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gwnogfqqk.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gakytmqzq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/grvgvkyce.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gvytjdtyi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ggdkyeltc.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gmqmbifqq.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/guxxurzgd.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gamjdkwhk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gsaunvyau.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gdsoqasoy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/glbwpxqsy.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gnnpqejtz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gkuyfjzsq.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gzzmmmmeg.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gczhwbrqc.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gxznqwagh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/goffvyixz.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fehbvm.com/Article/details/gwioydbvt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gtqbmqjmw.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gvsaqwkrn.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gezwkrsij.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfroypxcg.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gkzamqbfa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwdbzanjl.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/ghjrjpdwx.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gghjtbomp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gijmntuyq.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/ggtdeyzkn.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gralimmqf.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gjoyulyza.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gweivdqvr.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gnxqqkdgo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gmbgcywyh.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gncggfdza.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/grbeaghnb.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/goetlooso.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gvzmmkwmk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gjuwhpcro.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gjuwvurth.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gvhhkwyxj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gtxpekxyg.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gyvpjeeaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gfzbnoovi.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gdyfndebu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/gyragnqds.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gkicraubw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/ggbpojoxh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gsesuusrw.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkoonmegm.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/glorurxtw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gkokhyang.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gogtuthqa.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gddjjiqel.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gtleklreb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gtsqnurpn.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gnejfteam.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gjidaiwwa.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/ghkhpaisg.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gerhuyyzd.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/ggmewqniv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gvpmriphm.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gdmjschmi.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gighjatkn.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gibmmguih.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gwhgoeewh.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gczqgpfzf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/giitwlrga.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/guexlomzs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gkoixwolc.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gkuzqsacl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gopetlbue.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gydiwsmef.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gadkvcxit.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gcrtixqdh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/goejwgzzf.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gfxhhhbyd.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gzjuntrja.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gvtsklrsu.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gnojxfjfx.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/guxpgbopt.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gbllbyizk.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gebywemfa.sHtML


<!-- 参考信息 -->