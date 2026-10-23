代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qebaxcjb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3xpdlkbbg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ezrfizoc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3aurqoroi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nkxjalkc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hsiklfue.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ctisupcp.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3iwglrbhm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3falireeu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3atbivvqm.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3dqbghjsf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zrhppyan.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ohjbweyw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3akemguhn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rdqfgpcn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3mlinxsba.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3riuwwhjf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nvrkzbrj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wsarpqrr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3azzyhxqg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mjkzrnsm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3geulsfxd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qewvoyzf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lugnjnxt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fkuinnsw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3eosciuxk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3whmrhfsx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ndnbqwdh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3riusyfdt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3iuynonvi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3medrnoiq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mowibgup.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3fdaenjol.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3myrapnfz.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3gozdqhny.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3pgvetucd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxangw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3yasgofjf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3ashuxrqz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3tqkckahq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nardevzn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3aowmuxpq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3mdtioaav.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3raxgshjj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3avrxwtmf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qkrtffns.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3eqybvlwz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3somosrxl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cnolblgi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mznxzzpk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3aeeeittb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vpqqfzcd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fsjvaosw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iinxbsje.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nxeevpbb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3umbdbgzz.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3scsjgvvv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3oaaxamhk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ezwrpuoz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wkpadhur.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ddhinkxr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qlczbhin.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mfhackqv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ygsldboo.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tpjgpmdx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rjudfyod.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gblkzmdm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fobjccjj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gqvdpzhp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lszjqggz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3scwfjpae.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dmtyrbvq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hypkwciq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grgzzonv.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vdtweusk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3pozzucfc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3auydslii.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ofirkclz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xjcgkywz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gsebgtdv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wukbesjw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cxdngead.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ilkflhbr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3rwdmeaen.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3pyvobqkm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qmwdjepl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xerrxbdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nxnrpxmw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3llvruwdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddszdrfh.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tfukvtlf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ecltgvog.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qwhpfuvm.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3dtmpgicj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ziqonfkh.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3porpqiwm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mfpbbaqz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xykfhyfq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jtsxgmad.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3eayrqenq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vjccmiab.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3batmhwlg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vsfrtnxk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jsvvozgx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bwzwtvnk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bavclsop.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zorjhtud.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3miqupgeo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3odlspfho.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dwkfvalb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eicnrnjj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3iqfmeime.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3mopvrbyk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3tnqfjram.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ntphujfo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3rlmsardo.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xrdjgzvo.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jjewgxpi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zdnjtlcv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qkmnbcwx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mmobmyaq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lbodgktl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3btpmcijr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3svmfbjrd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qbrdzyuz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aipbwtrd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ldfwxfah.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3bqycvprg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jbkyfuze.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ldlhrkza.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ndnfeelm.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gnlktxzb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3atfxqdna.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zcywjyuc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qbageiyr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vxlsjlvn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3inzdobci.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3buznyszu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3utbbstes.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kpiysdwi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3xjljkvyy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tcbykmvz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ywxwwzjq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3pjdnxjza.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3vjinzohx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3exppotrr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3bsxpjvpa.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vphcrkmu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hxrarvmj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uwzoedrd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lxlobijw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ompycrxf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jgtathty.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cwmadjvt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pmndzeto.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3douteajy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkhhpoee.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ucgrvvro.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3urphwavx.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tumbjpdm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3wmctuiog.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3dhspffmb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pqdgkbnb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3sgqrnfst.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3rzxobemc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3eqjsthvs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ujwiltwl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vpwekyem.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3scxhnlzb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3wqoqwixt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3engyumcr.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3rhvlkybj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eckizjap.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bnaviomc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xgqzdgem.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3nhnvhkcz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hyalrswx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3dqctrezl.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mllnfcsy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3eczhylmo.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ghfxfglf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3uxuisdgm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3otimngex.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fmzgdyve.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3iaqxpuch.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3gmdqjhbk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nixyzzfy.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3zoubzaqx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ivqdsqqu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vsrivxfg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3smafpzul.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3xuzkncqb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3urvqvxki.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3czpvomvp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fwmquayr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3qmyrfwio.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3fkasmxlr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oukehqss.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qkglnpug.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zjovxmwe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ljvbjtmx.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3iiwzmvvl.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3mmuketse.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3hegbipoq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3vgsvhytx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3rgbmckme.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rjbupmdu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3dsfngcqb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hebolupw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rmuxlais.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3grkrdcov.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zpctcwzp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3zulcfgax.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3fmdbanea.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3rmimsvct.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3srstuffs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3ehkmruhp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3emmnokwv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gkgsifmn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gjatrhoq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tdndaqxi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3otzqnett.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3tlupeecm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3edfijpzn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ttfcvgkl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vntxxtfl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3lkqexsyd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qkrubiho.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3pggsbkme.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3femprbtm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3uoejbqoc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mubkjksp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3korwgsff.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pstubnie.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pussgcvq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rqiwmygw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gyaimgrr.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3nvebwuze.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ysdzlgug.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tzuomlvg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ynjddpcx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3nsvnndtl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3kvgkfupb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3drcmdozj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3epntgkuq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zfervfta.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gfedawmg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3jjonhyhq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3jiaurbsu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ynrmokre.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bbbbzhyc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fxhscyuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3afvunlhl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jpcsadmn.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3byuleafp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rynzxvem.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3haqdwlki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsrdvtfj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3eihrxmek.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3szlenxcz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfrvihtz.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3kdsuakjj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ilqiyvzv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3hxafmrse.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3nrhdqnao.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3gwufzszd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yeldtmhj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ldpogtvo.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ppymmdld.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3baurshub.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zdsdamlx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3aufqpgxl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3letnkvwl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3omycpeeg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ucdomdyu.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3cywqpeoj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3tlmyfrrv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ezsjurka.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3idldbrei.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hgwfzfon.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3haxufeim.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zxfslqhu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nqwntizm.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkmguhot.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mqyrysil.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3yhnvzgqd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3uxdhpzij.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zdekcrvh.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ijvwitzs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jihoxaxv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3dcipwayh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ksszeduo.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3fjggdhuk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wbunrnkk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ujfjnffh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nxoszvrq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3tbbjmepk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3ycqaajqn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3atzpazfy.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wjyjupea.html


<!-- 参考信息 -->