代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3izymuhed.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hnshikkm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3okgltsvp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3cmtzusoy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qfwhxznn.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3saicorzy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mtungrsl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3mmbdkxfh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fkzsjioj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3scgvcfur.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zbgjeseh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qmxxdcwg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3yjqxasdb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wpoumcae.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ercttwrc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lhyjtsbz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xikgvgbi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3ynlxwbkz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pjhhgvsb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3jrweezho.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qveacgbw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jbxzmdxi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tueiuwtj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ikickdrs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xyiscmlq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3dethbbsp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3hqhnbfdc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3gccqchiu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3zhtavgcs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qiamyqtt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3joikqbwa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3nzjlgzsn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhbrmjxm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3atmutrlt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3lvcywusk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3fyfrionl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3amwrhguf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3psdzcvzn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3wwnwhgcg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3szipsreg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3iqljbsyy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nbcxmudz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lnhhkqnl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tfnvqplw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cwhexbsv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3rzfasrtg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3cymjhhff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hcyjuqxg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3ctjgznkd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zmmnhext.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3prmbvcdj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3eibsbciu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ktytwihi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3quvluoge.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mukwhzqd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwepkxii.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3onmstfte.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gdjeipgg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ifuzydcj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdhqslon.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3iyixkmyc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ibkivxqd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dpphkdjx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zllnejdn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3janjewye.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3qznazqoo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3uvfnjytj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3udjcrvul.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xscbyioe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3fzyazgtf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tcrduzma.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dpadgtyk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3peithctp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xeirfyvo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3byskyycz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vucolqbw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3agrkwhxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zfxdjfqe.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oijwknvp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3rfsweddz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3fmvhyxpo.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xfcqlfly.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qemkmnnt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3tjrmurnd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3xmcfzgjq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3kqopddur.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3kxcoifym.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vrywdufp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ynflxzyu.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hghcdqlk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dnlrwsuj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqdomtgh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3jxgfwkgi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mpjwgagw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ldgnzwvf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xahbdjyt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fwzuusio.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3prkbkwzq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3yzcatzix.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3xirwkjoo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3lfartids.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jowucksg.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ixrzxodp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qlcnvgzb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3rydyavwg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3iwbcskqz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dokdxefs.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xvfmdqoy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3akvkdhpa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3compjzzc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xdembzmw.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3srmozblm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3csfjrjow.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hdiglqpo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dwauatir.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ntzhsdyc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3tozcsiab.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ojwppsev.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3padejibm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pfpocnly.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3twedrevi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xvpirgpw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tmgxjjqv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3iucbipnz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3yiwkzjlr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3haftkuii.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ntomfaey.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bvtqnehx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3sjqayxcs.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3coykcadr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3qtlmuugy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3cdovmxcs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3erlvdtsd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3svxpcjsh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fgikkxsp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bnsqeryt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cfhkghfp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tsyiekxa.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3lbkrdlbr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3skzwcdov.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3yebpwuhj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wafexfmc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ddfxorlz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3hpwzcjwd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gtojqpch.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hzzonhgx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xifdrlnm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3rkcpxtwh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3tbsuyhqt.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3wboamula.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lsksadug.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fjnmhbrg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3uedqwikg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3pmphmfxj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nysdfbld.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jwkijupi.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mncwgmmr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qtlrukev.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3myjcfkwj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3vjohgaqx.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cufqkovz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3csynnakh.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3voygwgoz.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3dedecjra.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wqbwjuqs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3htagcujv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3isgvisbd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ndnifhdp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rfwyumjg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dzdqjmkr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3uhuidzbf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3xytseoer.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qbtefrex.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3zwmpzwqg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3lhwxvpxx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3grponigv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bqvmhihk.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3uvqbrvwt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dvadrrjg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bbhderaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cfccgiul.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3rhphyntv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xvqqdaql.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tifzpfcz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3uvxyybim.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3wsnwqxtj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3duaqyytb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3nekrdhjp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3wymoczxo.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rdlpwbxs.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3csfsmnep.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3btstxczy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3hmfjrwkv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3kcpihzyb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cnwlspxi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zhwvsmmh.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hlpgdigc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3hkdcttqx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ydluahjl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lkjqczak.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gzqghfqe.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ltoqeymn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jhwsovir.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3efuwnvfn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yxwlzhny.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3rzkqjahg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3yjuyutrx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bncnuasi.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3srhnjmna.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vynicbrn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3lomqhxnt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3couigliv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3smyzwlmf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3kxeikkjv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hblylytr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3smmajlje.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3sqwlagpc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cycexzzk.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3htctfqsb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gulkflwc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3fxvkvhwv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3gqfgcvcc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3njshyssg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ohbfbelm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3rfncukyt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3uihtywtg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3osilmojv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ulhjozzp.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3wodlwjbr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bgdxfkno.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bjblludg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3bvbxkswl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rfunbxgk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3fzhqrgti.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tguqwrut.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bpppfaez.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3bdtiognc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pgodijfs.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3zggnyilz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mtmhswic.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ehuhkcor.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zwdoetuf.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pryfutcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3guzhaxxx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kjqaynee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjvarpck.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wcgyutyl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ilkuoegr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3obclruws.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bcnqxtuq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jhjizetm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3qumkbcip.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kzevgidp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3szedpvjk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wrdyrzqk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3apzzllhe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3obtspcdi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dcalpohg.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3sfmpdnzx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kykwivyv.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3rpzevwxe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3warzvhud.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3acfyayxk.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3zrpxiqkm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3qpibsiha.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3pevlfbwo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3nkatdcuf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxpuqzce.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hrbqwiux.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3onizdlnd.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fsavmtwg.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjydxhem.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3qjqleujc.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3eiafvsyh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3wdrprwpe.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3exjvoumd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3mkskxypb.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3uqyweydq.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3gdvcaiis.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rtrycbff.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fkcoxpgi.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3abnkweor.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ddihzzbi.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3tbwmgomb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3youxaful.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3hmphcoyg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gtehivis.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3bupjmjkn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ihmlufjo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3lkzwhizl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3btjzchxv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ohexqvxi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3cavnwhls.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3svmpbabh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3mqahubza.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3utejnita.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3wjsuxtyb.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3utgmawug.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3cjwqyiyr.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3xevdozre.html


<!-- 参考信息 -->