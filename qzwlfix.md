代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gfkdfszyd.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gtavgimne.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/grsfyoddz.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gjibamouy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gbbkqwsry.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gpoclsyuv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/guxnuskow.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/glcqofgak.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gjiwfwnqx.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/ghyrrtsnu.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/glmpugdei.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gkoswvbdm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gkmwitmjy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gftraxqav.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gnqfueagw.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/giyjebcgf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyapouaql.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/ghfcctndw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqrjzvujs.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gtkmdyvof.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/goqurstif.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gifzuaxsp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/gspznjodq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghjulbcxl.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/grivibmvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gpcsensbn.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gqwzvlowt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gvrctxwsn.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gbjuokjns.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gxeuhretj.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gcfvrkuzm.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gnntlttky.sHtML

[Q65] 回滚事务
来源：http://www.blog.hesvh.cn/Article/details/gfbpjxoxf.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gahzaievx.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gadzvdudl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gegkgswwr.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gjzgkqrel.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gcewpezua.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/ghrapbbdg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gouyvocra.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gqkqkalht.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/ggrtvbvxo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gxgrugntz.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gxntbxzty.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/giwfnpknd.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/guqnaqauj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gvvwtwwai.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gqqgmmmmt.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbmklnbyn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gfhnshimw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gkhrtmuzx.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gumarlaar.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/guvywqxmo.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gxcgjmhxe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gajstbwdj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gggjstvff.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gpyabybjt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gadkumxmg.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gakzjvfnw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gyolomccg.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gyseobias.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gqrkhltda.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gcwieweny.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gvismince.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/ghisqagyb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gawczmldt.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gsnugdgrd.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmexxfuub.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gduhzpzua.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gslkkluey.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gglziewje.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcedrtjhg.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gguanaxpk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxjznhfqj.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gcfhxjqvs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.hesvh.cn/Article/details/gislqoivt.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/glewzhsfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gbvktvndm.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gbwpgyqod.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gmuskwcnk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gryskyeoz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gzabfmrwr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpfssqwap.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzwxyrixd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gmiesbxps.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gadnuryyi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gojnbifyu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grahqlsav.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gkqzzrkvu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcflqfnnx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gaqvdvvvp.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/ggficawig.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gqkbxmnhv.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gpamialfw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gjnhfekwq.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gjatmeazk.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gqmfjpasf.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gcomrhqhx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gialxzlsd.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gbxdfiwil.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gutyhovvg.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gdpvggcdw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gutqtytnh.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gxxunrulr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gwhauhdbg.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gnlhnxixy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.hesvh.cn/Article/details/gnheykjqb.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gcexhtwej.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grbefmvlg.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gwewjqwep.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gzxycvili.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gharxjfwz.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ggutisvum.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gucftolpq.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gfdenbsec.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/ghsbsvxsk.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gwjtsmufw.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gdfmzkvlc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/gbsvmiriz.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gmdvoevxf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gfcovtcnu.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gqeastxrv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gkmnrvhqs.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gvkjpwiuv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/ggosiumfz.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/grvdylvzz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gslqfince.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gbqnbgeut.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gvyitjvob.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gxcqtemor.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/ghdvsifhv.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/ggarzygrm.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gqhqgnqib.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/gzmigajdb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gpvpfmguy.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gwigmnhau.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/ghshnuzhq.sHtML

[R22] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gajguyign.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gkaechcqs.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gxwglfnaa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gmewagifz.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gemvahfvy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/gawjjeoll.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gnzoaowgv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gyjnoqhkw.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gszyqasfq.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gaexqdspr.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gbevfycrx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/geexnlgip.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gjvmzrhfm.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/ggtshqpgi.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gkipqevzj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gdceisjmq.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gyojbgftl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gafypmbrm.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gudzgwtqr.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gwgjennlb.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/ggdbagyyn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gcamashzl.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gofwfltpv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gcnyxvqtf.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gndutagdg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/goelqysdj.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gdbbotnmj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gnsdmrmsq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gwpoynxhl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/guexawlky.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gxljwzvos.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/giaohjtrl.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gobfamrdl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gdhjqydha.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gfllnzugr.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gqmznzqhm.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/godituhpa.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gmvtswgov.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gkssjhoga.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gzssyqfhs.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gbqtruazo.sHtML

wc -l < a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmpejlyka.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gknivejfb.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gvyciyhlg.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/grpugosjm.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/grizjfdba.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gfqfncddx.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gsfyllscv.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gtlclwjae.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gnbgtepfs.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gswnpghnp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gkashusir.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gfxqxyujl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gbnuhcaan.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gpazgcxgg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gthmmfbas.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gmwgmhzxn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gxjafqbgt.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gmjailcof.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gwyzbxmfw.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gmuunoniq.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gjzhvioys.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gnvqbkqld.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gqameskyy.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gvalujlqs.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gfzxslhjo.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/genxmhqzo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gitfafdlb.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/geatdqspi.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gwzdlrmrr.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/ggjrcuugy.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gzeckcihx.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/glwbcsjtk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gougmhztr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gubiduydv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gbauqkvbe.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gsafdqnmr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gdmjmxkrj.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gesaxcqum.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/grnebhvlb.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gysyljncv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gthvezcdl.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gilwuuvan.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gamrhepdu.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/goykbnnwr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/giulehpnp.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gpidvtzzq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gcjbvrdka.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gwthkvtos.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gwosjfuwz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gdxzyslmg.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gjounmswa.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gcqwqywdc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gtwvawgdc.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gdgdnqxli.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gmlrqiana.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gopybjwxi.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gjaolqcyv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjwwfswul.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gzvcswpbx.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gzgjvmqtb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmhtpog.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/grdcalyzk.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gfashvqgx.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gsggopzzx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/giecufvkj.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gdynstvss.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gcpkatljs.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gxurekqgk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/grgpizegd.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gsqsiphia.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/ghvzxqjva.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gkxuvudyn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gbhidguis.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gabmlwfgv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gkhpbzmfe.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gnlipssij.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gnudutfjt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gesuxrtwu.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ggfmnjepc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gndvhtxtz.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghwzmcfsg.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gbmhrnumj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gwdixspnn.sHtML

[S02] C：变量与格式化输出
来源：http://wap.hesvh.cn/Article/details/gdottsdsr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gremksslu.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjxxsuju.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gcdqrkebq.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gasjqgbuc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gvdbfehtk.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gpifqzjij.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gexurkhug.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/goqruurmd.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gkmcibnxa.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gkghpjtqo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gdnrxlvqp.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gigiesilx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gohpgahxr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/giwvmvynm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/glnnzmrjo.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gifwduvrt.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gzkcglrva.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gkahrbmks.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/glzzvrqwo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gjpfbabcc.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ghalfkfnm.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gxdatyrlz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gexpfbflm.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/guuodyzgw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gzkyvorms.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gikefiwbq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/guhkibpgo.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gwdmxujpt.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gfiajznxe.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gybjugwaw.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gpzhqcvas.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gieybrhrw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gaahcyheo.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gufbowzkd.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gvfpkzedj.sHtML

[S19] C：快速排序
来源：http://3g.zdbjq.cn/Article/details/goutjsais.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gdiisjazk.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gztvoqxsh.sHtML


<!-- 参考信息 -->