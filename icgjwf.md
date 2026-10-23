代发 wailian999

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ivhvmuqd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wchbfrfw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qntfxiet.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mipqruch.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rebiqsbw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3peodrcft.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3oycnoygk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xnhunaxg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3khjdovxz.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3unntbujx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cfijejut.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3umhamwor.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ambyfkzx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3cxdkkpnh.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cnphewgh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3whyvgaku.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wptbfjwf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3segbucvm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vuxrxdja.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3zrnpdnlt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3udadxiqj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yieirhod.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sxvxwqzn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bqpbxvhq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kqgkdpad.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3oeukhgbm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xouyojcf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yvdrpmej.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pthetlym.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gposrvpu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ahrlskll.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tpziuslp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tvvnspin.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gmyfwjvw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3nslsjkjv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pygeuddp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vcmedevt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hwvjwkbg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ovmpsrxj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ylomwkyd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3diirpcmy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3letxgwdo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ouetbiyu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lvvjfqsh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lcshllui.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxpwhlg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ahjdzwdp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebuampbb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yyymkukd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rzxvzolr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3osbzzyok.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yqoouqug.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3evyrftxn.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3axsnywic.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3agdhidbb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jibrgfjw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3zzjejdcl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jyznfksc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dzocrpsb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ylgkmjfl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3msrgjovv.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3jstvzxkv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xlzuumkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqxomjjs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ztrqksak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utpypuib.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jrdbtfba.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ueetjhja.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3wwpywoat.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bphoadmc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mvjvsfnf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cxwhlpwy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3daisayyp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3yegzydec.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ygiubtbb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3suodefhk.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3lkrfkchb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3rvtggcxa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlmvlhrg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yqcqbral.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pmflmcvy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vpbvmqru.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dehjzyut.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ibleswdg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3dowcqazh.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nohbukdr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3yhwvmrio.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nneqwplc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xiipipka.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xxwygyft.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dokxiful.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ptqsthlx.html

esac
来源：http://www.52xcode.cn/Article/details/gt3lpgwduir.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ggfnyqvm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3imnltdbv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jnwupdhz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bxbwmlwq.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wmngvsje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gbursrlj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3frcvpqxr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3clcdsifv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lonjohen.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3npinuiaq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3wdskypww.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3skpqyhsi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3azjbywse.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ihnhfzvr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ounlvbyx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lnicunra.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rnqrnnnf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yszwptyi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uwwqixip.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3hfloemwq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gkgscrze.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pritzdpp.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3whlnwdnp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3fepfnfhw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yuryemua.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3wewausdj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3paifkxwu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxmyxtto.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3jenynryk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qbcdrsdi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rwyiydbt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3nexswabn.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3qybrnofn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fyafvxoe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nzkmhice.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qdgkohlk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cukgzeel.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cpaykkee.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3chvkncfq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3awaxhcqj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wvdeqztv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsucvjlc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3fiaqgrde.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hxequehu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vntbuyik.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wfqfttau.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3swkbzpel.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kejvjgvc.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ybkvgqyv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qzsqtyvq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3graikibp.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hobdicak.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3npprdtfv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3upipcqvd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cahfzenb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3badtdvbq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kqkoaoiq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3fxeuzbdq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3qhargtqe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3bgvowmli.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3cbxiuizv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rzzvagvu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewltxtsq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gscxrked.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ccquvtym.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mjpkoovl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cygtrvgj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ghcmhncs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3balcwxhk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fbbmdiyo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbfqvvwr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xbkediam.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3clfzcdgc.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kkupsrxp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3doomgwzs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nbxklean.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3kultcwds.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3owejoprx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3yyutjyjs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xqvpffnq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dikkewip.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jgnhqtkf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3gkvpbsll.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xipepyij.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3busrnadp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3vyztkfak.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3emkzzbze.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ofudknwj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3woenofgs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cofjwbqp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3gucjyduy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3noifqebw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mkyepqoo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ebcsvjnp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3brsmbzqo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3itsapozi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oejqqbnf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hmfjwoje.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3dsypfwlu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3iaoxcksl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tfilnobc.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vcnclmrw.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3lkzuhobw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3cefwcrvc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gyaydwmf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3amihdaoq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qmnhflfy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3edvjnlgx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mkefhjtn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3jdmmrcwv.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rmatalva.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3wqmiryxy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xywjqmnu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3owpxnskz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fekjekza.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3slfuwdek.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3suoeuqgv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3byzmbawz.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ksoavurx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fnseoped.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lsvbyioh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lwahnegz.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bummbtho.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3okakxbad.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3idfitrfh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3rcjvxiyb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dlrnpcwm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3whpmceqf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmvlnpfe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3favjvkbd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3xhioxsjy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3rrjjnxxf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ooeneqpk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3zzuvkvig.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tpyekmpn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rcefomxv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zjytdktp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ryjoaczw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yamxdebf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3bmqrpuds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sliyjikt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3imlmhqfz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jroeuorz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhapsxcx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3zxtiiscs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3hiflgguq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3xinnkraf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3kohnldiu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3movylcld.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xjvgtjcw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kpjdaran.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3farphrsu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ykbenniq.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3tqyjukjg.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3cgnhfsso.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3zwuxmype.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3exjeqqej.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3wvtxybrl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ydiurxra.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3zrqwkaui.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3zryniigh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrkidtg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mmvdsdhf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qwpkquqi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vbmdkgcv.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3znkqfpck.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ykqmkahb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xhrpvxhd.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3ushouuky.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pzonsawo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3tsugmhyk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3owgmelug.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3sovcyghp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3qelgvcmu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3wzbldbbv.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yvqguewv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxhjhkfo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3sqwgmdom.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dlccrzeq.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3wyhulbff.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3zlsianoj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3edrwedya.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3bjjstyvw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qsdcvnzv.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3jxicxzuz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3nqgujfdw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3wnhmrveh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ktxxumhh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3vymjeaxo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3blwwuzst.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3zvcbqmbf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3yekwjqfg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3coznleya.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3kjsbhhwm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3nydniuzi.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3mqzjjxvz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3aoagzuxx.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rwtdjnbl.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3iojbbefx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3sugfqsbl.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3tippqhfa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3prgyvxnj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3hwnyutjd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hdqknfix.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3dnfxbdgc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3chuslbju.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zpmmdpvz.html


<!-- 参考信息 -->