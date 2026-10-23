代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hwyalvlh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3trapbdao.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xidxgxrn.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pkoaaqgn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rcimxgfz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dvtpctvs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pieizcxz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yeewqoxj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3itlerfeu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3biavyfsi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tnywcnbk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dppkyvmk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fbujfctd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wbupncxi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ivzibrye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nmcjtncu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jpiyocov.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mygdavdj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yuonmjfa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3kqxghnss.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tzqbowch.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3pacecfvo.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kngswptw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3uuhvktnq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ootcdpwg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3icodxyfz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3dkgiulmq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3owgfizqy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pumivsvy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ylqnzaom.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xjzjfiay.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rgpzypha.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3amecwlrf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sukzmgjn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lxaaqsic.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tprlwdkx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dayeqofx.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3idwjeidp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3yedlzowk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3coimwvoj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3iaymochg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3luhjkcwm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tekqmfut.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3mxdggrsv.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vjlwbgmg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3aessemle.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fvcsmhos.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3noddpzyg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ndklcuea.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3grbuqwws.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qtjvqihl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ztdpdtrf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3plxouayo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uqdcvpgc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nxuidncd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rfhowuja.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqjvkxrj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fzvgujfh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wsxeeliy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khqznwba.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3sulcgbxn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gjgahxtn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3fahmydmh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xmdflhqz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rthvtkjx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rrcgobvd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ckcozyzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3msoliywr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3uylatzcz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mbqcsjhe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vvftzqib.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kbgtojar.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3nnkkxhum.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3iqkllczh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ejbydtxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnvojgtu.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ygcvipfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsmltklv.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3lxsfykwy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3amqnnnnj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nxaglhvp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cbiszbbz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sgebnwmi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3emyryuhe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qktbflkg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvyarlzb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wbejqupz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tcrzdsjf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3atwbuphb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dpiyrood.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jlemgcog.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wfwnfjrp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3bwicfbbq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tfpojrlu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wjisuizj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uhdkhmqp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bkhgauwn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3chjjivvp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dpjeuykl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tbikmvdo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3psmppcgr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oegghqmm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fuxvbrdo.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3loxuqact.html

esac
来源：http://www.52xcode.cn/Article/details/gt3klrfmjko.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkprjcsx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ivnrvzth.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3uswfncit.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tsstmnal.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3pftzqjjs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wpmdmsog.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3dmawifga.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3yuleipbp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3glwbhidv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3jkgwwptk.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3varhrujx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryugaagl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3dgdbgusq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yjshrfzi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hhdldzcf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3wcdnvlpk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3rnevedtj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yurefefi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqpibdlp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ozmhavce.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3yornbfkk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zbpfvsai.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nygorjtt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3esvbpljz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qofyqzyj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ogaccqrp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3apcpsarm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wazpcqar.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gqrdrbbj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gagmjkbr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iqtwauso.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pdtrfdou.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mwrbwdqd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dhnhlcbm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kuruojqz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3hnplxhuz.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vywvvhff.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3sxbhepyf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3qsqyatcc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsibxjyq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lkprtddc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kxkzkhaw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3wjjoxbjh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3errhunkb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nmxwiqei.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3epoiwgex.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pvicqccm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3lwfrwqcj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vecnlupx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3oeujkjut.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rawpmpjs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wuddfafz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cfjmprbg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ndgpzuph.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3sqvbrivf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cnsztpse.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zclktvdj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3mpmxjlay.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3kijbxdfp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dtnxdiwh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ybmvlptp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zqviqaba.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3obzhlmps.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gqqrzcev.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3snpuxfea.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3jetjyyro.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3letgxbnv.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qpzukaag.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3llrxmvvu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qlnknuoz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3wbjdfgik.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wqqxsjeo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3sddutdfv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pbkkcdrv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3iprjgmuq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3lpcyfiyp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3mwpizyim.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qiraycbh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3eszxwiuu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3huktavyp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qnvmbiro.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zweqvevp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tvpwzvzz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3sfduyiik.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3orjyalag.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3taaysknx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3htwvkfoo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hsmhkuip.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qtwimwdp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vibrakwj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3swiccdym.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bhsgczjf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhehwhqt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mdnwcdmm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zuwyszua.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ewgfskqs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dpgdwnsw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mtsrfgzf.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3iampkrni.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3asszswrn.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3lgenvwhj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3chcqcmuz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ukvfnral.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cevurqze.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jjtixqku.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3zovhjrmd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3bkcfmndj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3riwgayzp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3kfxvpsyq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ddbmahau.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3lipzrudn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yafugnxd.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3eqoneeug.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3iqvjinqr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3eesvwhba.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3cekaqsjg.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3tmwadxex.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3buwqisob.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zaqldott.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3blprvmhi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uoqxgrli.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eptafoar.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3isaphaqj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yyfoblum.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ovnlzcjy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wvplakss.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pqjhsccq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3steiqedg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ufaycmfv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mkfvpezy.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dreupkfs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3qgobtgwy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ghggtdyh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3oqzyhgum.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3lurvudmc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3atuxvpuy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bisyfwxq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3qbkkdlil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tedhhboc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zgqfdrhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnjhxqog.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dgwwtqsm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3lrzmceax.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ahfwtnum.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iibbynim.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jkkugjqy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqrihd.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3xsgzqmxq.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3gtfjuoln.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3jgbgfvbe.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vgyyfqqb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3arjwicod.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kgmebcxh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3rlypgnhj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bcwuiyiy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lxebwaci.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3mjoipvza.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3paepvfru.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3jygbazys.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3opsfyhvv.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3nciafhel.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pgepwrno.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxocwvfn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3onynbfsi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zfihjrjv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mnxbdoci.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3wwliviku.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yxvivndk.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3erquxxdj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3vwiqtwhe.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3lznyuqyt.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3cbhwbgvt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3jxsjhurp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3mwjktnie.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3nnojviqo.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3txteresu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jiyxfrve.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3beawnerw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vlpnqxol.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ynwktzxb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3nrbnyjjs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3piqkxrxt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3onudvxws.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ddacprpj.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3lphlpmed.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3nwwpardz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wzzomfvm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yucmbdar.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3vmlnutya.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ecvblbqd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3qaltwjgi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3uqmkzxzv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3fdxxulnb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3ulbziotv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lhazhvmt.html


<!-- 参考信息 -->