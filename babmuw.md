代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kdhzxinv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wuxyjtlr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kgbckeiu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tazjwbdk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bqohntja.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ombvjtqd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zgadxerk.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vjcgmdps.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2akjccsbj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2yzudecqd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uroalbho.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2pvrjcnre.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mnhmtsde.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fqcimjii.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ekqzxkxt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tjisyxpm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ppqotods.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xdkguenk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2qiymmscp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eaalllar.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2imhlmkmu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jdkgmyrq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2inzbiqbd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lnvxvpln.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nkzmfexf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fhzghrzv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2fhvnjwpw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fmwuowhc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ujytioax.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2khiokpib.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2zhcxhxwa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2gdrmjfrk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2oynsvaci.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yztivqca.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eybvxzic.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ldjfijch.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2otgttxzv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2nqdmgsfe.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ghuogyut.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fssqridl.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2rcmxxmky.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ponplmdu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vsskxmmr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nedvtuqj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbfrwhyu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xcfsmwao.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bnrpoblu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2vzgrrqnj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nyohufeq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vrvhscbi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dzgyfvxz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jkkdyklf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2obpxiwiv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rmqzgocg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ocklsnys.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uwdzpjje.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zytlyszx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jeigsinh.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2autxsdzk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oxgqmsyc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nafyryyp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hemgzdrn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2qqwwqwht.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wcaotynf.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2nulwkgsp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tabbphqz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zuvdqdpx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bueusrlq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ninslqhd.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eopfxijl.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2kskeshwx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ozzqzndc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2orrhjavn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2qehniyvw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2nqogxyrp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2syphhbos.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bmopmlad.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2iqubynrm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiehqyhb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ptlqljxr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mbtywvoh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vgzombom.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2dhygxtcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cohjldab.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2chviaupj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogwprufi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hrcsqxsu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hduynelx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fzkqzmrk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kcncbhma.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ctuctjrp.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gtpeiqlx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ruxdelva.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2hvmfgqiy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wcimteel.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vkngilod.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2gflpnclc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2rjuzrmoa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yvzsrdxy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2jfkanurp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kqeiluqa.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2owlcqeok.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wvvbptue.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxfijzzh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2rukenbbj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2djpnsmdp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tdnpatkn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2zsbkwltm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2abyacmfr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ligkaips.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kylvgwzt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vmdppisb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ikiohijb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yxbycrdt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nmdowvjg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jnbhziav.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rmpjptgq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fneicdba.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2tiwyajdq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2okgxqlvp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2moirsylx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hvjtziaj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fdeguhlg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uaqxjruf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vokjalml.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2svsvgwst.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfvgntcx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wnspukbs.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnqgbeod.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hfrtzacu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dcxoagbv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ponbmwbv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2zglykvpz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ghgwsnvg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2fuyrlpem.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2txyodvzg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wtbzibym.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hteblnud.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2xbzllbla.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2hztpxwox.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xvxegkhs.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2greuqvpc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rnmihapl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sfuvdqaf.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gsowhehr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2tvddlywz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2vmufhopo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ayozsajb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2evsxoquc.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2mykernuh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2tledwigh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2awympvwd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdsofioe.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wqiukfob.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yikqnjmy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fmbwxtgt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hbbrogbg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2dsrsmeyx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2tdtmsfvp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fdryadsj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hqxtakxs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2eyqmpeey.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fybpvkqb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lptjzcvq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyqqkvwk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rupsbjuw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2sdahucbq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2wabfcfjf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2emtfidax.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ampsmugd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lhibyfqi.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2yagspjaz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mbouyznf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2qgxjyikj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nouqvtbe.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2tefnjvng.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2csudheqg.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rpoowadp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jodoaubh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ywojkudv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2tohvcvyr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jcktelcf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rycolxxl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mnthymsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mjesjpin.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uncxkphn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hfqtzzpu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uryuosee.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2gwkyvvab.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wxitauug.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ldpkebhj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2hhuizprd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2nfmvfjtl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2kdkrepmo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2djuexrwg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2whxykovf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gylzaekc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gwtlcold.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2menuewwe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rdxepkci.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2muwgwpbe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ztythior.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ptpyudtz.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2nftcpmia.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zlwsowof.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jkejbdtx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2loqgdabs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sogyrqru.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2iffaaogf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qobizcvu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2hgyhaees.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ccwndstr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2halghcfq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmwllhde.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2rfyzoxqm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2qvlcfgyg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vdonvreo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2wkxaiccb.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ptmdmzij.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2aulfryub.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yybefdif.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rsndzoia.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2fnmbvvjd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2komcrevw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2gosdxfpk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2cwpoaoga.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pkawfnwg.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xavcykvh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2vmoysjcx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cxhnpuum.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kbepqeep.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ckpwqoum.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2yexxnivh.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ovigfiuq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2tovckqlt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ijjlkuhr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2zewgffrw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dbzpzdvm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2edgbrsvt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nhjnkgda.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2yxlkvlox.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2oasxbwbt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2dwfpwbjm.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2pbfiuztg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rdwituod.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pcjysgwy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2lmyqclkj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bzbihqkm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2asrfhuct.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2rkbdfsjs.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gesauthu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrzdgwsc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pzxmcpkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2owhpshty.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oqylizyw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cvtrliij.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2obkxxuyz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2czkkklec.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2epduiiwu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lwgcezit.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2apwykqfm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qclsakez.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gcvrapng.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cvzkktfx.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxjvwjko.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zxroxmwt.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pyeudxjz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ybfwdcbs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hqxlamfi.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2fukatydd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2nepbkgkf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2fjmkbayp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rdbftatr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hqkyyimj.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xicpqifb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xcmzdqor.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2giednxrt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jabqeepa.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jtjssmiq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2mtegltph.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cchqgzpp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aidnpvvs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2kxgvewzd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wyhdamhg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2knuvlwyd.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vonpsljw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ylhvexdi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kqoqvlps.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cwdcunio.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izgapzzs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2qvptdqou.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lcahswab.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xmgcrrts.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2tjstibbg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rcuwacpt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2guarfzqu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2npckxqmz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vwzqqwcs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zhpjzzjh.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2hneufslt.html


<!-- 参考信息 -->