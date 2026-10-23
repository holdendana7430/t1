代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3dcuqbpkv.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3tjmvbbgu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zeurrlkv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rjirqepm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ahrsvdkk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xwyjbdmy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bujpqdcl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gvsmqkeb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xpslsafk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cmqqjrln.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gffvldop.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kovwwzbk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yljnaopg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3cuxlvuye.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ylkxdyyt.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vljejyas.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3niiqvmrf.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3vfisjuub.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ychebgsd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ancbnwoc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3igpxgcad.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yimrylcc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3hiuufbjw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bwcvkoxy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cfmjgmej.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ptxnkqvn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zdosvjwe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xnxjugma.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3jfanzuso.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xeztmlpq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3lxsagrwq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3aqfnzogf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ywyzgifa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3bersjgfn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wjwgrjhg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3dyfxzryl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iajkfbat.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3rwfhsixx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3qbheerug.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3reownqiw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3fcpzczai.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3brnflavr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zkvsoqmt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qiijcdcq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aunvlndw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3wqntyotr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vmdohfdl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3uqzpijse.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3aysagadg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ampfvksu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aebgdwvz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3vpbfsbjn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3aetnuxja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3nxvsvthu.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3snkjyesc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kosctrmx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3imsuckpm.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xozlpnbk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3edniaobv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hzwmydvf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3lgghipfa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkniispk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fzgrkdof.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uiqyvqcj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3eszprexo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcfhprjo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jqlhihzy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vzgaojse.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3oyrvnwyf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dembsaaw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mzizbylq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rshhnklq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zrpgblki.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3odydixot.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3aauvlwst.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ndswamyg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bezgoxab.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fcnhfxyb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uwcbipmi.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hlsqsdwg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ouyqmyzk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wmmhdfzr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qhwjaedf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rittswjz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pfbsbucr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdtkkueo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ejkhaypo.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3sgwszykk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zibfeqox.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jqsbecxu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wsfwetds.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3yzsoifus.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cdalftex.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ixwvsita.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3febffwyp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xtagloqh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3hdqyfqmh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3eszttgpl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivlgrgqs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ezsqvarv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3uzebesxl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pybvsiva.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qxitqhjy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nouovxbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wnszrcfp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nmreyidn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hvljnake.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fnhkhyjv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fsipsimv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zhwndmkh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wfrxpdch.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xvgnwhrp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ayyrftyp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyceryqp.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hconiskx.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rhzkybxe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3clydvnng.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3tkvlbznz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3owzfnevw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hceewapy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hurerikb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cbtkoqdx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgynmdtl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hspeekop.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iugbqypi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3nslfnhye.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mtprqlpr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wfuwlaoc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kyawuroj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fvntczmq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3jelxoiws.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hjdgtknv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fzatofkp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dlkucuch.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3otavavap.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gfmhhbow.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3vnokhdiq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3semidxuk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lypkhluz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3syooaept.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3esmcsihw.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fqwcmcza.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3isdtpvya.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3sosgrdsn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3hcrvsdhp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ogplmjzy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3yvfglxyr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qnyjlixy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ereorjme.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zdjjijkc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fzgssadt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qqzcqtlh.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3byvpdkin.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3rthnvzda.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3whqeucaz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3nnfljiun.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gpncjsto.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3fggpprde.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mesarqin.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3cbscoyyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3lyeiteig.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3nprwdken.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tevmonnw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3virpfzwg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhwjsujg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gyqavfxe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wbfhwbci.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3hgyykrxm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3stefzuyk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ctxmvbeu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3mscrpslv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3peiwppav.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cjhcjptc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3hqyovcqj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3cakfeoif.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3errmtnnt.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tkeekfdu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jzwpdnwb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3amcaeilc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ofydtxqo.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ehblmmuh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3cxwezlqv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ffdbynyp.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3dkhfxhww.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fhmtmncj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vekhhiup.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cjzoeqdj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3lspgvepn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3znjqspsl.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3xciqcpqv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3amlbbtqi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3shqoaxwh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3wrjnvndt.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qvntnirn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zoqlnjnc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3eawjpwgd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3vfcjpyfu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dgyvmero.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3agvwdoan.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nyhytglb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3xkhqurda.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kvrtsbbj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bncxexhn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3hhokahsf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3jsgtxbsy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3iljmnjfd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ajktirhe.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3elbmyzac.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ndcpkknm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rzzrnqge.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3kpakdblw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xdkvnrbq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3szkzdybb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3mmuuuxph.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3tkfikium.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3cnzptosr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vxyxfiag.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kdjedyzp.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tajwxhaq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bbmdprvo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ofttnpos.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jljdbmss.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3guzlljas.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gagheqau.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3epgfappi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bfwlvueg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sgmekhhn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wovrdwwp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bogpkjbr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ectndljg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3czaxileb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3imxkyxlk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3puxagjvi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jhepsecm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fpsydtde.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3oedbeeeh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3oxtkneyl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3gljtggmy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fxmgnnqw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mwwfacog.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bceqjfry.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3tgxeuopd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3seklpwcu.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gnkoiuru.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3etsbdiby.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3gueegcfv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zcklzpqp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qfkbpqnr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3qxurhhwo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3aqwohjqx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qihvszhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdasbtng.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3qqpqncfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maqkwfzs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hhsprjpz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3qugaaphk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixvluhth.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xwgayxpi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3iksmxock.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3iacjgebg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3epxflgqc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3fgulfjnb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cpdpxtzu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xfywvwlx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lunqraja.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dyjszkdy.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3xemyjpyg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqijak.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3twgsrfyx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3yohvhwtw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3swjlueeq.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3uqanbtih.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3dnpqnmls.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3ccwctmzl.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3vkygjwwm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3foexevam.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wfffrsde.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3plyfgide.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xokynoqd.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3tycugmha.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3zrflggrl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3qwzytevi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3dshsuyqa.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rfutthfc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3apqmjrjs.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3aqegobhc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3jadsautj.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3mzwswkcl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3pkjjxtka.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mkufoisb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3oshmmdpf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3glpueezx.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3oyhypgnb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3mtqmfiqu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3elrpnyij.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3okwnixgl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nhnhsxim.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3rylcqxdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3mtndmvaq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wrjgufpp.html


<!-- 参考信息 -->