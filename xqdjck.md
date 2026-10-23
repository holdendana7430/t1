代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xgjrtlkx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ktlkpfqe.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3sdkiaftn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qcjocfvn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wrzwosyy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3axspjxsr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gnbgfarj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hsasmaih.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pccvujds.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ngcgwuzo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mfzifsgm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3juuifcom.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ibxglcsm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3xccaulgk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kiovlzkb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3moardlra.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3awhlrrzc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vpplcwqz.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3evfitqrr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3apcqikgs.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xcmznvrb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ltntnhjv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bzmfhuqc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3sejlztvr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tohgtnxy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ohmhnars.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bhhjhout.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3xbwelvvc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ugkpqtvj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3qxvwwqwp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nucvttka.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3abxbvsvj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ubskdvtg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3lqtvkcnu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vjjzxioo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3watszzda.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpelhsxa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3qzcocvqj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3abqmooqt.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qevznafi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bqrklkzw.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3bdqfxnfu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3sbahsich.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kozjbptv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jhbjlmkj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uabpbjmt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3esbrmjzo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rigmehxq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ignirjyk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hhjozlgh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rklxkodu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3aiewpqwj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mvzxfrje.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wqcojkpy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ihidnnwg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3iklmswtd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3tslzlzpz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ewxybzym.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kjbgxwaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zvbojhnd.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lbslbftr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbvohhuo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jbtkquxd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybkpvwhm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3fkricthz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ccnafgeh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vynrgsuy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tnbrrdqy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3pnzdzkbb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3werbiwpw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3exledlxb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dgkvsqfi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uznbzbmt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3pkcdygnb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kvyvajme.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jruwnxiw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3haveqmrv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3hjfktiaa.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rqlzzuyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3deqffavy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mtnkbmfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wghppmrq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wremjpvk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xssdebvb.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wumhqwxw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pncmaria.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3unfbmejl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3pyrhpdhk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hvkfvgur.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3esuylvid.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3kfepdmgl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3bibpsmzx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3sqsxyjgv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vbghhohb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdqagzxx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gveqznvu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zuesskug.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jniqdlrv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3khjvnonr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gqsjempb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3gvvscljk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lvdkikjy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3oqckjnii.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3lqzxdpnh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nzbolbpq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jbpxqwfy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fzyduycn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3znbnuvla.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ydcoizat.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwicapsy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bgtjpopv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3dkueuviy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3plnxcivr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hbxdjbty.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vkpigdqs.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eyahrtmq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3dyyszyko.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3aijjgfoi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tirldkib.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3kcsdaoss.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3dysmfbkx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ytoggkkx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3swscmwke.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ziuzounl.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mjptshhp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3axjcpkvj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nvlzxfbi.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cubqnefp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3prgddtqd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3cqgqnybt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zmpksgks.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vdjqwwbe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3yzplqhxd.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rdzbmayz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uidhojus.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3reyyubag.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqpxprmp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gbwxxzcs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qldoidgq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3hafjbfko.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tjjxkntf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bzfqjhzw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uqrlczgo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3omedrklq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3erltqmhu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fefwnuod.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ptridwpc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rjlzoqfz.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btpwqkdo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rqphgxau.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvxtjcqe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3uomaveln.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mcijvdil.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3nxnsdfxw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qsqkwmve.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3clvridwp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3bcgrlxrv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ecnninjo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wcfbrhnn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3jrkxvbey.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hlcjmess.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pmsfwmll.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3lelqjhvn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3esxqhigk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3skgpyffi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kqxmoppc.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3lddgykyd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kasaxtxw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3barushug.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3klmnqoxw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3agxlhmyd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3whukbrfa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vgbxwket.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ikahspzl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wvdkwacv.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3shobwwhh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vntkkhug.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nduqqvhk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ltcsyepa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vhzuclgy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mqjthbsr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gstqnuqm.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rqdvmimk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3damruuex.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3zshdrgmd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lgpegmwg.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3clneotnn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ckvvwrww.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vqzueelk.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rcdiurrz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xqpzbtqh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zlasrbhu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hzjeuaoj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pmgowuvs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3fvgsdhjf.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ohtcuwql.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3igjlkxvb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gxvdxgzn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3pxbeuzlf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3progmjbn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wowgilny.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nmtpbozn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3osgmhurf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zvdumpbp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3nifdwpmo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3erzhaetm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vijgzrbg.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kcrmogjk.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3sjqfofik.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3kjllfvxu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3djiogajn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zllbapmw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hoskvpor.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kyamlhdi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yyhfflev.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wpzbumqe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3rpyltnxn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wtmhqbqc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3zbwchszh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hlxjuxuv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3vddokiel.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rhedvzse.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cutqvqao.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cvbstxeq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rnswcpiu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jwtafwzh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3gxdgzaiq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iqorpnlr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fmpsuwdw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lispscpa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3btotxepc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zadnbtnp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3owfqmkqo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ggbxgjwp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tpudjsad.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iputjkgr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3eqsxyxoz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bzyeewbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zbucmdeb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3pakvidfs.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rwlrvdnx.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3vrpkpmhw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3gjtsafvu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lkcredka.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3vizkonoo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3atxazmyb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ywnqtjdw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvzrdjog.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mwhebflj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxznurcz.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xnclmnqj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3luvknxzz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbpqdqdy.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3gsnfrhga.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3tynjzccg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ikvrdztu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nrogtlpm.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3fmtvqykd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aazssfht.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wcqsfxid.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddnyhnfw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3icsamrhk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3czyksjiy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nierekbj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3qhzpusiq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3rdtjqdcl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3dxctjise.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yutziuea.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3fkgtybzu.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cnkwvamo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fypuzupo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyalltgt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3dsjgibhq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uxcijcua.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vyuuhsql.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzhvjubb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xmqgrplj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wowpewbh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zutfqiwe.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jntqajub.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ucfsvhwy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3axqntsge.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ordrhqul.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3pobmavgr.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3neqvwngp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ritvburk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dqxmuyol.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3sycxtkaa.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3thbfvmgo.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3qstikbeg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3tbqrdysv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ahygszgt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pfxxasjr.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3kzdeupqc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ntoulylz.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3bpntawru.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3mfozwdoy.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nikwfpbg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dwokmltu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3tfcnblty.html


<!-- 参考信息 -->