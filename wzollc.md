代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nlblcabw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yqzupitk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yamxuftr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vugvwqts.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2apojqijm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yivirodt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mxhjbeyf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2favilhkx.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xbzsfghs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yttcvxao.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fmxjyyvh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2whkjiilj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2sxlbirbh.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2amrnznrn.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gralgcgn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ogttbuys.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mwcfpkvy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2nvowhawm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2uxsfwgns.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qwpkxfyc.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2nlckqzon.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dhrvpqun.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2elinunrc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2eisnurcd.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2kbqysmhb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wgajkxpc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nwywznxm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ozbzbddl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2azoiasor.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xikuefis.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2eegcbyjt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hlloiehj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zzxawlsq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xauelcdj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cnylwzct.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2djoiewuu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2xskvacnk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ehchimad.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xapqqsbu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2glymlhkr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mykgpdol.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cpxasuhd.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2obynsijo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2zjsqtprd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2iezektjo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cfsvjjis.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ayifngyh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqcfxjhe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2npmuwonk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oarxhweg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wyikrmol.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwuhtrmb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2vijbuqwf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ksggwepw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fryyzyfg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jglesztz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lvnfqgti.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zxndzlna.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2jotbkxjl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ohdsvaxb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2swhxzlii.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wfwvjzuj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wyvdqfju.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2okpdcbuf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ksbzhrow.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2kimijifg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qaqgbwhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgxdvwtn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2igaqvqio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vblpowqq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2snzyymfm.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xkuhekkg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2ianjtyim.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2oarpkzmt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2sgnkmjyw.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mhnowpsn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2njdhrzau.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qilxinsx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2sxrqttll.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dzzjrriw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2rcreilwa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nnwesrax.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2atzollyh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngnqyaim.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2onngicdc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dzenoqza.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2aghoaffu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2enfrxbjo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xxjsyeij.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gizoiciy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ctxoaldb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2kdwsihwa.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ydtushvs.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mcdkasax.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2vmwcchpf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mlnpyhkp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2gabavduc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xjcuaywe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tasdyygi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2wymngrlv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tgnmsqlx.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2miquknui.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cbisjzzo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jhgjztqt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vbxzdbsz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2atoonqhr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijdgwmnx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yijainav.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnyewexz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yhletqae.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sqojyjcd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dhzaebdo.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ohuzojnb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kemdpzuv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kasdqelk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2sojftbcr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mkdzybes.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ixyndqff.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2agnllfph.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dfqucpyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vacgqgdh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cakjsmhc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2gmdwmnzc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2czyjofco.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2oordbrjg.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qdpmdcly.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2smqyimdg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gyvexmtg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ktgekqul.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cjdkbcaw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hmflwsib.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2glwueovw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dfmukbhe.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ucmmlsnv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vqxgtbey.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sxlhjqoq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rexniuso.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ouschcrd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyhlxqdl.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2pmgpswdo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2rkfhkxcz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rhvsnelx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ioognreg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zkzmulmf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2aaiofwdx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2boxvrrmw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2oxmldhzn.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ekupphtq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xaorjutt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2thfuvhjx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2uivxyuuo.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2duyimfme.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yksrpigb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fywacbto.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2romwtalg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2vzctrjpe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mjsmumhb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dhapymno.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sgkcrnww.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lsirejft.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xvhfndlz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hyhrsduu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ehaxvwfa.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2gphdhwcn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ibaeslqg.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gsszsjcc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ipiqssax.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgyohatu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzrwkyrx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2xeczdvae.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fgetrkfj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hvexgmla.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2obhfvfhg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qqlpoapb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lvzluqux.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rkbuqlxl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vqtxuggg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qifdvmqv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2wlbkmipm.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2eccmjzil.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2yhhbvzpz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjlenavy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2eegoebcj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ucvvyuur.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zmasmyzy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ridesayo.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pkietpdq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2czcumspp.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lieqpzqq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2hzwexwat.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lufzudev.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ysoxxyyq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ocbimyqp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2mitwtprt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jrhmeugu.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2flihncxm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nuokbhie.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2lltvbsln.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2iddbbiwx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ukhlbmly.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jgrdqalh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2zpyzowhb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2bwninjvr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rhocpbyr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hqxltmjy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2omzavdeg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2zocspiwy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2berymgvv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2haarywff.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kgaxvwmg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smxknwxe.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2lswokktd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2uxqqkjuu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2metjzbxm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xbikvzis.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nmdeptpj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2onyftvln.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gqxbkerx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wnjypndm.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rohbxibi.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nuieorrb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2xowlihqe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2pqhpfbwk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yclqxeoy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2neytxqza.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxyglqli.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2witlnlgl.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xkiaflaw.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zfyzuhxr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ffeidiwo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2rtuozfhs.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2igsegckk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2mscyzwzh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xnlbpbgi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2msbjtsru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hieeujzd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ziidmsxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujzsrzpn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2catquxir.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2khrctqje.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmvhyomq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kvranqfo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2vsuwucgg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tusafeeo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2gdthcbal.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2yxgzukhu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pjyhwvbh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfrmspux.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2eveloxbw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qocarbyr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2bhubefmv.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tdfgwyyu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2yphwucvm.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wgtachav.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tsorcjbl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2nuryboni.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2oymycpes.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lcsqfsii.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2exzurkne.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcfqoqii.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2nmpnbfdo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2bwibafcw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2lbjhluje.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2bnorhpik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rggienax.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2cfvhwpaa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2msqexitj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2doekjapc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2gorpqebz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2orddpfgw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2irjshasv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fyrbqquq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2cxwcxhir.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rqjffkxv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yfwygume.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2madgisiy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ybpwnrms.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zzgysjnk.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hhtyydil.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dgdzuial.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cquqvysu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2rrvtrise.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2xtdqwfbe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rwsbuekx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2neswgszf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mjqgpgre.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wtcaiedh.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2krojafns.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2admpztyd.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ytrlnyec.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2gktpxvjf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hjaapucv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2zsglwuuk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2umsiwfbb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2orkgimor.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kmrrxzgk.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2gmdyliot.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dqufwkcq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tlamopts.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2thtkzmbg.html


<!-- 参考信息 -->