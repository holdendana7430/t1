代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bmndoxet.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zcizezag.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qefjkmfp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fwuepdpv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vsroduba.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2ajnymcqm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oiuilyvx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ffrhyhxt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvsrrzrg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2cjdofuhl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zcckvdbp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2tstpizjx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2abzbaswk.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2vdsabnkf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2qvcmhato.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fuhexjgt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2wtqmqxqr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rbuvyvwb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dukxwpyy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ecgakqxn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bfnlexcl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dtdjhvwe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2jajnunnh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kcdclutl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gicicvrg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jwgakpjz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uvgqfinn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2jreuecqw.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2wvvargst.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wjmbhdai.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2oljelhvq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2plctumyf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2rxntbysj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lgugqqwy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hkrmxhhl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mwzbfxjs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsawctyu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fmceurfw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2novtutsf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pxtycqxm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rekbwbri.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2putbvhgj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2vgugyemj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2lpmhkech.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2iirpjkqi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2sydrlxzh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xmoagjtl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2oitiuqky.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2capnkuws.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nsrqardf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2sxmvhuxf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2iljiuvyf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ptbrzxli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2czsfhnfl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2oamlnhsy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kmydqfee.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2sjnodrao.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gdyzeckp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mcrvilpr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2avjbdthb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2iogmaagn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dqablrwf.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2itfibxqa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2crmfjkll.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ipivezww.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2znniluht.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2cwkjztgv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2swrmpnlb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qespavno.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ywngrjkr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mmhhibok.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xrxevkzp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ffxjucao.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wgzgizfc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xcblejhe.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hmambmvg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mrktveyl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qhfhwtmp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yfcrwkps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkpqbcbk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zusxjnov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmgxwhce.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2uxqfjazr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kwdiluzc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2slsefpom.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2qkrpwura.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uekawgeh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2coonbdks.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tswpvvma.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yrhjplur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mcnkmxsn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tswacmpf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2plkirruv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2vvtinzlm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gorzhket.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vvmofmii.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uagcqxsz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lgffvglm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lbriuzsi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pngdjhkv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qegjeauy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zasqhiiz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2twucprhn.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ptyknkqh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2srbbpxhy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zthsnkck.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2dyfdzfcz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nkjhvics.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mfgrhhul.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2teeumyzx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fogbewlc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2niezsvfz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2thusehxt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ffaeedlr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nmmoihgp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yeqaskfq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2iggllnjz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xcsmczdo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pvfbycuo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2dvwdujww.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2bysrfnso.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wuuelnbg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ympihhxk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jpdakhua.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2uegmwqiy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nvnvtfjx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2msyjlkyx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fncceamu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzcvxofu.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kibkloum.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yrbqdlai.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aovjekuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2kphgzlqk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2sqemeblq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qgmmojxq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2duqiwiqf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2bmwliuqk.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jcuwnkdr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2dcrwaclb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wuxmfdxk.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bvwalnpw.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xpybogqp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2otcadwmt.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jkoeokgc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2swoagbms.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tibwjslf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qhdeclip.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2mvrhroqr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qikhamao.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bdsowdye.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bfeoicri.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2iypimotv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oenvljzh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rniqfivz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yzokzsqt.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2yglptoav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2zjygkykc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hlkjwfet.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xttqsjdm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mswbpskp.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2txtaclfu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2prqlffea.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gxwomrdj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bxxwfkuz.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yunqptpy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2eyjmjjxl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vufyieed.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ikmvtaqr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kchleyud.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2eglubrid.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gujmhdwy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qfswjyvj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2wwyeunqj.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2izhehlmp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2bupapsvd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2esqinfbm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2icxlfuhz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ytmkgfnh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xaawfswp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2uyglaplg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lznsmkdq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nkveceua.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uwxwuwye.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vajevgky.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2bwzssbsu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uoecqmvy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ndiaccra.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2urawszcs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2erteykqw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2sgblohho.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vqhnzqco.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2svgvnqqn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2uolacgbg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vprjogwp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2atjkzgwd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jtbpzbbr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ckyyfcpn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xbajnydh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2idpxkmyx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2kxtvxofj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rxfzhncl.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mfusmhjb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2amzvtawy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ymenwmjy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sskozope.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uuqnwipz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2njeiatvr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2tsnqphpa.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gyczhamf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2swemhfwx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2loqpjgml.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2svgzdeck.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2cbbwixug.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2uwwvhzjw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lepdnjrt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2krhdekhr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lcnrjjnw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lzxwntea.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2helckiqh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ikgmfvdx.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kqmhcuzr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mwusfixg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2jfprgbyj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2khgahoco.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yxknjixv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jmqpbloa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hergqiij.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rcdjufbq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2eruunsas.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sqdyqvpm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tkuzvias.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2uagsoobv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bmfefziq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2drlfnysr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eibnpmgu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bklrfzdc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2vmzqpeof.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrjppolw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2oznrcfnv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kxkuaopq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2eduwyorq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2agbespfe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2lwfblfqx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2lumlfonx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ajqaacod.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cxpyvvvv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2wgdmxucx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzvqtuvx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vkwcqorp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkmgxbch.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xbepslqj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lkwhexjg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2udlktjzl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xnwsxgxv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gwvfhovg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2hkexfdtb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2vjgntody.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2doefvixg.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2aovoameq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tkbusbfd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2noziabup.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mqkceasy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lwqtgudm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2aihropxf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ybhexzyn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2naudyers.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2jiwsiant.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2icoygjzc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gsrmihsy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2bxhszkzk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fooxphpw.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nqcdiuzk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ovoczwjk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2dhxsrpbh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mopasdzd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2njiwnxwo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2iynrbrfm.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2alslgaie.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zjpvligj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bkspmoug.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2aaqhpuhm.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ferijril.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2rydvcmof.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lpoiuahu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2klvbhrhw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2njitjptq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2zxpgjnxi.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kueurcms.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2maqkourd.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fksmyrwy.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ytuqzleg.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pnzixfrq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cvkoslpl.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tquokgtg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2joohvggw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mhkqzhlv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2xysvotit.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2dpafuwvn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkdfay.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2basjzhvg.html


<!-- 参考信息 -->