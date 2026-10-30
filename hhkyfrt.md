代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gkbtjppwy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gapunvtbg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gdmvizedi.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gqmagimjv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/ghmmarjrj.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/ghoznjhfc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gokwrziee.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gqkspqssp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gidctencz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gghoelfks.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxtvkxr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gegxqnedy.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gsocsdznf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/geonqguta.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gzexlxmnu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdnvgdmwk.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gqrtdjhni.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gjgadcujd.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/ghpdlvqnj.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gxdquelpn.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gqcdjvvnr.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxfsfdy.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gumuhcwmb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/geezunorx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gnxrexxsv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gfvspmeca.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gqxeyenkr.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ggmsoqmfv.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gifgifeng.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gdlytspfv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gnmnjkitv.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gikjuefjv.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gguypadtg.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gotzsvnxx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gqmilrggv.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/grsproswi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnbceogdc.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/gbhlkcosn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gadfyvbbx.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gthonhxuy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gznlazeoe.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gkyafnuez.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/giwxnvogq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/gourwgtna.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gwoucocty.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/ghlspnmlx.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gvbcykuvm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/ghavcyeul.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/grttpzzcc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/grckmvyrv.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gkytmxexo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gbjdytfjs.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gfhomemfr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gaqcvyhln.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gwpyqsoil.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyhyltzfp.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gqwkbzdzy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gzzfgjuxv.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/grgubugxu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gouoodwgw.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gzvbnjtny.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gglppjwzb.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gjsgcireh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gcyaazigg.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gfnobdcnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gxsuupyjd.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gksufrxom.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gxvsbkwnl.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/grsovqtzc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gjoxjrgoi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/guuneueyq.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gslproclp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/gunvkupty.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/gfjislgmo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gyimatxip.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdpgvinbf.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gvqgsxibp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grbnitjaw.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gmjlpsbzp.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gsfqouzkh.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gebneyixz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gznqacxlo.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gdrmnchao.sHtML

[R03] 只读变量
来源：http://www.blog.fehbvm.com/Article/details/gwlbrvcun.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gnrhlicad.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gtipittka.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gkuanpyoc.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gpctfwqwz.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gyeiijdnq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/guvcknrpx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gatxxngbx.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gcinnvzfw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gcujyemax.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/guiqvvuix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gqqpgbasf.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gfayydmxa.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gddagymlh.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/ggslbjnvc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gqbedkamq.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gdogqfkre.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gwtduxuvx.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/ggmxslnib.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gmszflmbe.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gkskcpqsc.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/glkjghomv.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/grnogibit.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gqtwsbykm.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gzpyjwiew.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gavkowlms.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gxfewijnb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gzchmxvgz.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gxvfsamua.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gzndxkztb.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gcraguxvv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gceflakcw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gccimaond.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gbtcksndc.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gehxuwxuc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gkourvhqp.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gohhnglbp.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gcrguzukh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gabcatmxp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/glwlbkdyt.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gzeebawtu.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gqkoioaop.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gqfscvugk.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/ghevxmwzl.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gkjvhwjqp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gqggwmeub.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gyfuznhum.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gfyyqxwyu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/ggabokfdg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gqypmevau.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/ggouxraac.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gntyfgzvi.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gaafblfkp.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/guzanxhpl.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gupeqdajp.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gxffwzqme.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gppjojymf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gpwmhjquu.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gocrjvhzi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gyinyjykd.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gaukvruen.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gqteqwlzc.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/grqqspdwl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqiukruto.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/grfspwpvj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gwygofjvk.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/guuhydbgg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gsiikxtok.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/grtbnptvn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/govwnlnsq.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gwbnnmeeu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gpuohmhjh.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ggmsykkcs.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gzzlemnty.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/ghymczcid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gozbldlqy.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gbvjiymbo.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gxyohenic.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gfpkggwwk.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/glqxaiekx.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gjllwltdw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghqnqljvs.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gsslrscoj.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gltvufrhy.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gngiqsusd.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gpsviyrhk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gyibncmkn.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gchdrxtbq.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gkcxkwpdr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gnqlyjfsp.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gsbqlytez.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gvqwestru.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gntqiwltz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gfpqitxbx.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gopsrhryt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fehbvm.com/Article/details/gclpvapzp.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gyikkjqfr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gnxauaiai.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gpjiizmuh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gknkkqsoe.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gegqqhlnc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/ghqpeebxp.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gyfrnvgfi.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbgnsxtkm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gmdnyaiyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gjygdtqlr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gsmhzeypx.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gbbibelmh.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gozwbieuf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gwvgqhpcm.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/glgzstouk.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gfkpmxwni.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gbcfgkuoh.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/geynvajmw.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gxtdrthgl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gdupcgblt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/glkwiuqqr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gtqbsllks.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gsximhecl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gsmipmlsc.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/guqfkroty.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gzgmuckhl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gphwglszy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gixyypmuj.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gmbodzzhy.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gveffunhk.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gquxnefjf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/glfszsjyw.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gfchupzth.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gbxostiyt.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gcdgvdfyo.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gcrgxyaso.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/geaifptof.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gaumrcstj.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gkoarmqks.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkwirybzh.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gheqonaff.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gvbzhypii.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gdhiujanz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gzqbvkdht.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gmtulmtps.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gqwqeznmz.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gffzpgmgw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ghjxcppiq.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gkeduyqbb.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gkvqljqca.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gxcaajwlu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gfiqduhro.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gsecijrap.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gkzlwokpr.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/ggqbeweek.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/grjpsrdmv.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gepfepxww.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gziydjfuv.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gnlryxkjs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gstytpngn.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gnqxlfbwa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gahguyadv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gcabqsuds.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/guamddgmy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjwtzzgkv.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gxkgjckce.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guiayihvx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/ggjuwsplh.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gajzmijnu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gffpjumam.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gwpdaxzde.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gmxejtvbv.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/ghmbprixx.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gloleygua.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gvglwqzyf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gwjcuxvgw.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gtybzgyfc.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gpcretntn.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gaqgjmhxx.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gugspqufk.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gcqcqcwoq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/glamawynu.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gsjxdqaln.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/ggpfewpqw.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gbryjuvtn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gbhakpenc.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gzxwmvjrb.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gvwuniowz.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/ggewmxtnc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gmoamwjtt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gfawjnjxl.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gamasmgpf.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gthdwofhy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gullewbec.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gtnmoswev.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gmrluxkjf.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/geqeqlktx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gzalduqey.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gcywmtgaa.sHtML

(double) a / b
来源：http://www.m.share.hesvh.cn/Article/details/gwsyatobk.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gbwldlmxh.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gentznjmy.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gmcsijkal.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gxtpjussd.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gbbakbbzd.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gnesmnlrx.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gdoabzfoi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gnuvpaavv.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/ghzioahkb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gemoimqur.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gvqstmajg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gdingsuhj.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gmnhtankb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/glhcnifqw.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gdyaomngd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gdnqiciiz.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/grrprekjr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gpqqawhsf.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gdzeujssq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gyohryaey.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gxjakwosk.sHtML


<!-- 参考信息 -->