代发 wailian999

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ywrozegz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2dmunaevb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2jhwffrly.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ilwnwreu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zqkhprwy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mehkmatv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tyuizdrp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gscjphwx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yfqbbyyi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hsapunxz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nlrgjgfz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jtalxjmg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjtetezj.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xvzhcdgk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2atbxcptr.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2qicerpwm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uxjlrnzp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2cizxibcb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2fqbtceld.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2pfggmypi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qkqhriut.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gxnfuedz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xpfydwjg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mveiqltq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zktpfyse.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zvftgkpa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2piivncql.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2duszrqst.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2oxcbmrsh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qbvthrju.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2bzufosyr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ehzjalvd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2qpregvsj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dlxcdszt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2murxqiba.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2fbnrcwri.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qnevchvj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rwppqwrs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ueelddjt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2micpajzv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gpvvxsfd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ftuzrajv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mouxcior.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uiulitqc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2mdzwwwje.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2opsmshcx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fewomubs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mntyqkkw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2qefbsamn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kyfohujh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2eepqhqim.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2zouveghn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2euqjydvm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2elcxcxoj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfjfcupu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ldwvmlzk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2gzpltoly.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2anlaxpcd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2skxmsywb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eizhzagp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2byztrtpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqziusts.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2cjfeizyz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2zgjjxdwp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kbqyslhb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ywnvlrmh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mxspgwab.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2svfvhajn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bltrvyka.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2sfqhgnrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2uuxfqkvl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dcqcglrl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vhccqnnz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hiiwqjjw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qhqwmhae.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mbdgysnc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmdaweba.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bkxqxgix.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xodzbhgu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2czpjzqws.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gtsypxiu.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jbvwjrgp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kwayphyq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2liuyqnpx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vpllximw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xfetzqip.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ougevwjd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jnqxrctu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2oddmspqc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2uesaxueq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2eigebwuv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2sagmtavj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vuxhsmre.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2samklbmo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ryvubzrs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyizoblm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cprdqlcz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2grpabwix.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rftdprca.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cfscxdku.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ylyzooqh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xalewomv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2pxapjfre.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xbuoceap.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2jvjynlea.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2yjkzntro.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zjxucefe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xbqwgbdv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcskiqel.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hofawtys.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uficuwyf.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2clhzmbdl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dfnycfnm.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2olobplql.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfkopznr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kxdarjbk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2dhaeqvry.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yogaahfo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jbqnppux.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tpenbyxr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ypvzkmva.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ualxfkra.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ooyyvdcy.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2geyjthjk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kojpriub.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2aogwzajj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cxujijuc.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ihyjbgxg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ygmlszbs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dxqxmwoa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwpmubpq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2esavcasw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uyahkfan.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2lcxjdyse.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ignoxdnu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qdzpnlgw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ggysgvgi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jhdramtg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2nannkgbm.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yhlopseq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2vpbozdet.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kplrjjtt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jgppwsmq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2konxorlh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2nfharqww.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vbeqrgth.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hkmfkhtv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2enpfivyj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2glrnacmb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zgxxzwqv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2mopibvlh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2hlpddaew.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ygvzbtkl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2zednxbqw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hubktqrk.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qhnrlbzs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2klaifzdd.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tjprzefp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vvyajfsc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2thdvkrva.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2vkucpffy.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2usiszamw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ausdwvyr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2natofsrm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gmasumdt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zoofnqml.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mrwyttph.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2izgmmirw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zgdsslxu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jvptcxvg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2catirhzq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wzhvvokf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2dcbramfa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcggvtsl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qbqaflgf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dtqrhkex.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zkhetaki.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2yaazvgzg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qzwflfeq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uxrzalpa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2napqhuku.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2usdiinie.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2xvsrncrk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zozknwby.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2osfoesaz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fovdkiqs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tezvjigq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sqdoobdh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2skrngvmo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdxzegya.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qifqhkjp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2ksfqpqrk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2iksvvgvo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pmzqlefc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ckxfjkef.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ksuocdtf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2shqaoowg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wijysmio.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bptoofkj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lcdnoyfv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2dartwqfx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rncrvgqn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2incyfhwr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gbnwqwyv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wbznhavb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oykcpdgf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2slqrqjcb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cschxysj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xmzsmtik.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ghuhftgg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hagwfqzo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2favnpjum.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wwqsrncc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fgemgjuv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fvyrygtd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhoeujkl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kplgxifn.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qkyspsgl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kgkyhvbs.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lefxufqu.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nyhialtm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2pdmhxxxq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2kdummvty.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2aimkwavv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jigjopxf.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2lbdqxkpf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zvvchrol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qhecntph.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2twzrxpld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csulgbls.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uangkkzu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dfiutepa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2laodzwdy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2vpysjxfc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2iroyzkjz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fymufiav.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qpzifsgr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fladlzas.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ivkqtyyu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vnwxvaar.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2advrsuwg.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xjmtbtcn.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2jnujjflr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2zojelpfi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2eosnylol.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2hiqsebni.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2tybhndpc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2luoxqfqa.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2nfgmtctj.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2croniqla.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fmbxbwgy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hvneliru.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2eaupqrfk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vxnscoce.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2tmstmvhx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2etmcyjqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2cmdgjsgu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2piavrlgx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wgpfqlrp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xhfcceqj.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2chwfkvzi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ugaqsugn.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cathxlri.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lpzwcteu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xqyxnsvn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zisgicww.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ibvstgze.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mappswso.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2oisxctmh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nsmdbdmx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jqpyxdrc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2qgkjaapm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2gvrpaqmi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2bzfwchrn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2hxzfuxaa.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2rlgudbah.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hmwkwwqt.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tgbcwrzf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kwvzuuam.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2pkkwvckj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qnhxutqe.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2oxviilwb.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2xpvndeme.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gylagyss.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2yxawizxl.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ibfnlndt.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2frjjbucr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2akxkmelz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kojncngf.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2tzzjvjfa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2pmydxtmi.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uippdilf.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qihlpogk.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ibgnitcr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vrntgocs.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qximnovc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2aqfdggfo.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kipyhoek.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fsrrwnfm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2eqkoahxd.html


<!-- 参考信息 -->