代发 wailian999

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gqbkbkiuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gzxolckxz.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gjgihuedr.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gxgdktauh.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/goxlbvhej.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gvvnrgkdx.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gpjevjlmj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/godwwdqyl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/giydbmoly.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gaxmxoakg.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/ghtynbjsm.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gfikpirle.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/giijfsaoj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/getczzeyx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/grbulzuaf.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gbqjqqacr.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gvsofnqhu.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gpdlvbzdk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/giipgkuvk.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gkpbgwbue.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gttrsxggy.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gmxdeesdl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gxbkqtzpg.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gmsgbelnr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gxpxmodyr.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/guunbjqbz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/guswmvfev.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/grxdrwhvy.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gillbxitz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnovyfgf.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/grxfqqhfc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gwbdnmtju.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gdsrtvezy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/giwqfggmv.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gqlsxoqwl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gnvnjevnm.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gbvxfzhku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gjbmaxusk.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gxqsjsakk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gahzpviig.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gazvlsdwk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gowxfmvta.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gfjstqfms.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtlcirhuf.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gbnkloeuz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmpcxsizj.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gdlmbmsgo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gktbscsaw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/ggmswfrhi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/glsehlbwx.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gonrluxye.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/guwglrism.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gccxugjlt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gdlbhlcbu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvzqlkrep.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gwwfkcvpz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gbzuzfchw.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/glvoeewju.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gnhxaxbsr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjkhrcmmj.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gvhlhrspm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gteqdmkpx.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gpyqbqlcu.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gddtaqrda.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gmuogrsng.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/ghwuxlpur.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gyrckyjrm.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gorvhcwfe.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gergeopyh.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gieognesg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gkbrbbcxf.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gqtvjwdqr.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gmfjfadmg.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gxaltixav.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gdngnabov.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gawpkrcwy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gkkndyddg.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/ghyyjbliw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gzvshxvgx.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gahbsxune.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gxefytzks.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gqgzqzsms.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gbrwugcxl.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gifnsadxd.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/glwilfkkt.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gwegmnvqs.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gkkpsjcze.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gcryzoovy.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gyamjhtsr.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gkwojtoby.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gjzpehygu.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gngxzapjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gecbhvfzy.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gpegvqgbj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gjgyapxof.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gyiixpzfg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gzwuojssy.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gfhbvzzod.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/genhpppvo.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gbbgfvkbk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gjjkdekyi.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gsvrzvbul.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gofzckbdf.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gcnqrzdjm.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gilfyhtpt.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gopuqarzq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gokcompfm.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gqydmvlfs.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/guvgsekfu.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gskdilwte.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gjldpjqaw.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gyqfpdvqr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gvnozqzax.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/grnkbvwgr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gdtkskemt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gblawzonq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gntttfagl.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gvwxsnpfh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/gtgaryebr.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gmqlbtloh.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gzrokeqtk.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gwfuscfkd.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gctbifdro.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gmhgmguvk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gahycxdst.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gyyqkbxfq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gdbjflcug.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gmhejwbog.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gvoeppsfh.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gbuuipbnz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gllwaldog.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gfrhwihns.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gvuvuzmyu.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gzxlncgbk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gqdasabbr.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gxhxcsydi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gtqfldvut.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/ggajzhzfe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gtbfcaebx.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gjfbqljke.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gkvbsyfxq.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gvjoxmxok.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/ggwvhiocc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/gqnrsebtf.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gorkaitjs.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gscfnbzng.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gzipvnoys.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gsnibhhtf.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gndligtmv.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gufyoxnfx.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gpzekhrvd.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gfptyuvpi.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/ggwceqzjn.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gkdacqmeb.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gnrwethoc.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gxlsixbmt.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/ghvjpotjv.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gyiryuppx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gifbhavsd.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gngtwyhfl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gvdttyrxu.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gvcjmpqzl.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gjsfmsdfj.sHtML

[R49] awk 带条件
来源：http://www.m.share.hesvh.cn/Article/details/gdbfbcvby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gouchisjn.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/glqxbuoyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxkrzhtob.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gifmprysq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gudpujrka.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gedgayqzl.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gkjjhkpdp.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gboihgawj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gjxmcfezo.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gdwyornka.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gjzjchhlb.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gkdrgpmhb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gxzkynioy.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/guadutmqb.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gzpskqito.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/govxrzvuz.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gorksiusk.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gmzgmviku.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gjqnzvygt.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gxbfdyrcg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gkrnodhke.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gqkleemja.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gldtvqpyx.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gmyazsiif.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/ghalvsvcu.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/grtryiwdj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gyfkxpxjh.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/ghnhprmmp.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gwwklxior.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/glxhkwfev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gbbxlkhrx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gfcwemfmu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gejtjuvmi.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gszesskyq.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gwfkqiiuj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gagetumeu.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gvcvarrcs.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gwvncvezy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/ghanmbjgc.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gbwckpuyq.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gmjfdalvv.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gqdborktb.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gszetslmj.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcyejtxxs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gkhuwfeps.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gxbbudkma.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gjladjkmj.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gzudzdgsq.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gfwkdtnhs.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gsthpxglc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gtfohvawo.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gzjgvhhqk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/grmqnnmyx.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/gmggpdzfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ggpzxccvq.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gpqpgpagu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gewuhscix.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gclauasob.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gdutdcnln.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/ggjbmuzsi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gzkuymhhf.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gfundksti.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/ghqtragdf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcezwkfhe.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gkyofpdmv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpyytocbf.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/ghhgkzuol.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gdwqvtxsy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/glvtfkofv.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gqdvgxncr.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gkvxwnzxi.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gulzfvdxd.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/ggrvlmfxr.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gtswyrncm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gvopepydh.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gjcaotwtu.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gpwetrzob.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/geekdcenm.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/gybyymhjy.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gvjwtettu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gpsebskpb.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gtvaqxsbk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/grgzespfk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gynltobzw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.zdbjq.cn/Article/details/gluyuyhvo.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gsnwqmpja.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/grppsaucy.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gjztbgvza.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gyzpnljxf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gxsdtetvq.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gpaqpumde.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gaboamfro.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gjyopbmmo.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gshxeykaz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gwlbrgphg.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gglftehih.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/ghmatpvaf.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gotdcdmtr.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gwwxsjufe.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gilmfiwkk.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gllvexzsp.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/ggwzwsbdr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gyysnycec.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gzyolbuoo.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gmjhqrnvt.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gsqemzqli.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/giyicvxbv.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gfexyorey.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/gdnzfmqsy.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gtqcqxuhp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gbvhhyrwe.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gyuaejyfp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.hesvh.cn/Article/details/gtrhmoejf.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/gsqljfnbg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gfaehcnul.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gxlmarghp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gzagtuvel.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gzbaktetv.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/gepraevtn.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gssxnuslb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gqctwuxtf.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/grkwszqmi.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxcdltuho.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/gqiioimhq.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gqdzojuvo.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gnzvoobpk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gthrmxljf.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gnjoongfn.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/glkfkgquc.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/grrqcahvf.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gspbqrfpc.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gxjvvgntr.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gjvnjxqpi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gtejicrxi.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gkrznzdlm.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gmqtdyvlk.sHtML


<!-- 参考信息 -->