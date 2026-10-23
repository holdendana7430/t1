代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ksryfppn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3mxnzpyjc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wrelclzl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jmjqbhvs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wlrvyzkr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ouuywfbj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3agwxskmm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3frhicksv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wyrnbpmj.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xiyxejue.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3dksrldys.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pdkfisgl.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pijszgap.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3bmxwsnrk.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3awsxydjw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3gjwzwxfq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3dbfwtwtt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ugiijfwb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nuhyhyod.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xgzlrzxt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3qeyuhkna.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3wndlomwn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3dmbhpwvi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3vrdhllje.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xrsneewp.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3pbjscbyt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ngetkrml.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fladfgkf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gykmmuto.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rqpddyvn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3efirgnht.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hgolptet.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vwgwnwro.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iyyjvdqv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3apgxgdkt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3sgaijjhj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqqnab.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rlxrhylm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dzbaicvv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3rkcmwidv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3lmzizspw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3fxiqgooj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3olqdzvhz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yadjowae.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vpphnbmf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfvwvtwy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3uwqxqzox.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mbfmidvm.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ostnrhdm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nxwunmif.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dyonnpgw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qdiqikcb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3totjbmrq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cxvmmqns.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3spqrhlgk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ojidkhui.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3ihkbihhl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wpsbngjz.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rqjyvdzy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3kjqiyayp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3omfnabqe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3rbtuuyyk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zoaqeqdc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bnejsvca.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mkudsdyf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uymkatox.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zadvquvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kszdpqdz.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ixaxpmjs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwqmbbcb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3exrxibpn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3oaqahqas.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3pqptkwjm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rxjxrexf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jxlweskj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3oflmhens.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3otjsgjvn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3nuojrpvb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wzblezsc.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jzqnyjip.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3coznttny.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mmkrwsyk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnttaeji.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3joacbozr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fhsxbhhs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ygteyist.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3inpnhjmu.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cnrddyla.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3yytuhxvi.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3fahxehco.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3msabsiwt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3euzvvhcu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zzwrcfqm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3llwaltuy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bsattkpt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3eqidvgww.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ysnwxhav.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3gnwrqevq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jisyjihf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wiatcfyx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bordhpfm.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fljvokhx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lnmmrnts.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3poinbirs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3klbxejwl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3zwcygpdf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmivwgpi.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3outqitzj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xbmrszmv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ebghdqhv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3inmpqvqr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3efgevxzm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gqjtzqoo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3eswyvbwl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pbxifpsd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jfhsfltf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3oytkxdam.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xbqsgwri.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ohlcckjv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cmaqcqht.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tvgwsiou.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3azasrhfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3shmbrldf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3gxhfpcbj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3tsbzsfwm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3iizhwcev.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3lzznbhvb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ufesdbtj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rkvenefu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ihrwtudw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3mvvnjvcz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcemnajt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3knxtaxip.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qyfbmxdi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3whhzqpve.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3yuozuakn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzoinha.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ebjintml.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3bhmajrhc.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zvdqdigd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3txofiefm.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mqpoqlkp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ztwjwfqk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bdtlgafn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3trdsdtqq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oxnhveqt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wasnuwbz.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yfdqdads.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gpphanyx.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3fpchgctg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3szdlsxci.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vusxrvzm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3udbduuvn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ebepovco.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3atrtbqpx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wnwfmvpx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3jqrafedi.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3wgeldpwr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jixistrh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtjjnhgc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jxnwmzqe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ypdelyvr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ctjdpvur.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zryjnlnq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vrdcbyly.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jzzffgmy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3edqasvba.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3ylwcrasc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3desfirve.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3etahbefx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ukupleri.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hsgjfeab.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3osckergp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3olcdwijo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wzmgbqnh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3kzftsjip.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lecoukes.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kztmgibw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eqiutqhv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zfnpkhym.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hyfhprcu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vtuyhorn.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vhcrhgnx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qvjkicig.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vytohrjd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3pjywplyv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3rwfqtyjf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mtlxevrl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3wpoytxum.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ujzwhlcy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3abwumowv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nuqddxei.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vunumolf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3laeouwmk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3tvscbosm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3sholqczg.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wnapjipf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qeaocgvx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3mfizsxzv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ameednxl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3uncmgalp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3agfwaeuo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vnyacttq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhohqs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3fncyodpc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ngwjxywl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3gwjxaccw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wmfwkqgu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lkcjeeof.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3gcdyuzro.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wqtdvgeg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wvogpizr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xbvifaoi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3efqkzfgx.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3soiipkoh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gqpqrqfk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pnxzcrlb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qncjevnv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bxbyjwus.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3stbsjiea.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3uqxqhwaf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ityywzfm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cvjdptpd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxfxhvag.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mkwikrus.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lrycjzys.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qwfcsgro.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lwcwicix.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wgfhdlxz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ivllqohl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3giocziha.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tcewlkis.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3btyktmkt.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3owuzdacr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ghzvthyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tedultuh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3uuzkukxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itvqjvso.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3obeygyna.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3yawhfvnr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtuorykc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sfmaheyx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3pqjypjwc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3sqpiufdk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3djfujqwr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3aifgotcb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wbqbwvvk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3clnawcre.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yahqwmjl.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rvujpkqa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3niwbyfaq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3skzfuphf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zcelswir.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3eozcyihq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3oklqpkxj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3vkxztgii.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3gnidcdzr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mqsfcgjq.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3cgfndrks.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpovlbza.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3vnjkpsfv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3kxxktsxb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vmbofuyx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3aadviedd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3payyaxqy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3afxemwjl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3esqljlyd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3cjtthhzv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3wtxudnsw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3gmvswrvb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3azqafeop.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3jptuvohb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3lofmndln.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3homtdyoe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3dngduokn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3briyvrmk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3enbspgol.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lbxjmwfx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uxvyibyj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3thkgfqww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zgxyhjuw.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3mvtzkvdg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpgfoze.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jwyeatut.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3iwvujvvp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3kcwemssj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zzgcjjcf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fgmdlxvt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mwumssqx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3hxdzibfy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3gfsupxea.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3atgfynir.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3qutprqla.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3tpewecco.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ebxybzhc.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3mokcinsu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3odouyjnq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3vnquzisk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3hcfgskjd.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3cippmcgv.html


<!-- 参考信息 -->