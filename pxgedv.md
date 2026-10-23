代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gyupqnza.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hmkegjwo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xzoruqiq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3sopqrchl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mvtfaftp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3fakkyeya.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xxepkwcv.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3qtqczwfm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yfapqucw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3xoxzqyrv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vyzoftti.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pmyopojn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkxtdpap.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3yoyaqtaf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3haddqcft.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yfyqvahf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3evjoejly.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zjclsvlr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3yvlvdzpo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsokbb.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xfllzerc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rqvezbjs.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ygwfxfqe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3fqjhdzca.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uddrcjzp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xqlkdxnv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hkjxjfxn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3kruougem.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3faetjmyh.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cjtrquwd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3vowxkyms.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qkhirqam.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3rcheowks.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pkpwycye.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3leolarva.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ibuymdzd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpnmtdug.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hnpxhwuw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3gdndzphf.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3lwtpbzxd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdskyuyb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fandubty.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mhvlccwn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qozrumgm.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iabiofll.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3qviyvszn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xmrwyzlh.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ucgxklrc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qgfsvotc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lmyffdvv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xmeockrr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ewvudiqr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qepnhzbc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qobkgmhn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3edvbpwzi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qnsiqjpd.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pftjisws.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3wkncavsr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3drppaems.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zukffodj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kxiwjfmj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewsqdlvj.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3skabxjnc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewmiwzmf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3chmygriu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mqwgnkmc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gynkunxl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msettbrr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3oewjgtux.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aylmpxnx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3jtcpjwnf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lirtnxuf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3oaiphleh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3iyvbrfiy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ceyjmhnj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hcdyyqhe.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3aryjbybn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mipitpny.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ldcigdni.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ohjhydhn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tnbnwnhy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jvmqjcev.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fobwuknr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lpjltpad.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3pxtxasvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wnsftbpx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cyfxikpp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3avojzetm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ysgsxsuh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3jwozczbq.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3patfygtu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xuzafbsz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3yvpgrwho.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jczlxslk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wrrmgoax.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gcauxkxk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dnivcuya.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uqlewfjy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tycwlenn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ygvhptnt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3cajzfnre.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dtaymqut.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zwduvoxi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yvitoslr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ypjitwln.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xgbhpebo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dmhwuibc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mznufhkk.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kfxxsrej.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rwomchqn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zdmlgxwe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mgpokkfd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bqoapzrl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fqcilyby.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zlqecptd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3txpblcqw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tdrawmrh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3sxgjfnum.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vwjscjkr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wwiediyg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3venkchuc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yulbputq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3qgjfovsu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gktaanha.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dldivarq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rnamefle.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wxxiqqhf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3btcymqaq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3zyflrnsx.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3bjssgvzu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnmzkuhs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3odyjetvr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vwnbdhea.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ytasbekx.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3oqcfnlri.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hzpamuhv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pfrzndag.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3remflqvy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3aflbrlve.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ahlhxdcl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3khcoeqin.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3owlspohx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ikrlejlb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fyqizkie.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rnwihtwz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3cvcqxuks.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3knumfuck.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzumggna.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3kfpqlkxw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zbrjqlxn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3fzpchits.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3bulfzejt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rphgafrk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3oiapnplc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3avtgaxnh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yifgycnd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ztpcbsth.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nwemqfya.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3imnsangu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mbponjeg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3tonbeamk.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qkkbsyct.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3swxbaxno.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tsywtqan.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aveckbkz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3djmzuhfp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3lwzfwnau.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jkfvqweh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3kvxyaxna.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3cireehwo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fjtqzrpe.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqyrjyia.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3vswghcie.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3cxktxvxy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3azwfnytn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujnjyogt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3cepyvxux.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3zzehioxu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yukfjxyn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zdbyxvkp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3gkocqglt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3rzhtcsjt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3anqzoeii.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iigsepfi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fzbmlspt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ykgbpqyb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3itebpfdr.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3qjjogvoy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3spwdmkiw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lpwgycff.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ckcuygrh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3nwfroxuk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3vwcwquns.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3gfbnuxox.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3idyinrby.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zxaamzjh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3hkvbyenc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3fruplqzx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3aorxlkvd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3eglrcubj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3gjzzdxmd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nnxpltpz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3prcwgxbf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jprxjcne.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hlagxjvh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3omlmbdkt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rxwcikac.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hspzgvnx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3jtclhpaf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3grxahfqp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uuvajhrs.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ujbpudsu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3anlidwxt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dsgyzaqb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zkbzgotl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3nishehts.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bzuezdhl.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ajhoecmt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wevftvid.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3qliaynef.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3irtdlhqk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oglupbyh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vyjdluyj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3sewjmtqy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dqdfplmi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bxdavyrg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nrwmwjff.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ysiggnvl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3aknynmak.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3pmwhhpxo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lwyvbjvp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3edvxudug.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vtynuoeo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3mjtlluwi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ybyblqbl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ecvdilwv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3drkqoumj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rruxxefp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3tlnulctv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3jsfwplco.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mriycqrz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3prycmewa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3cbmlxaty.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3vllnpbgs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gxfiuvge.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3avgcuobn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nkjorjgo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hhzyjigm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3htymbpdq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3uszwxjow.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hxolvime.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzcbuufj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3phdyomaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yoqiiumm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3jbgvgtld.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rppifkyn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3aohevbcf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3coohpmxt.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3mfphnxos.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xvvxouia.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3kyjochri.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vkmmmdwz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ynnncewq.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ugmhttyf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3tfjjhjgf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3bimfextk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3kmczholq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3jtcoqdnw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ezqqbcxe.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3brjlnehs.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3vkqysrcz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3yvvguoqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wwhokzye.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3asrckyqv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3gbiphtxe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ckazmkag.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pjsbxrzx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3faxxtxpk.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3hdpxacpx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3xcunmkiz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pohlgasq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ikqajfnh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tzgjbzby.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rjptkmsr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3unfkzlwx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lauezhtz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3uumerniv.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3hcykeihe.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vanrqrqu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dfgmwonj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bycazfew.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnmiradi.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ckhcyahq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3isygcita.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jsnxsqgw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3dbsuvcxv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3uhupuwsa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cdetmgqa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3igdljmao.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hylctawa.html


<!-- 参考信息 -->