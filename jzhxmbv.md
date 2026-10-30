代发 wailian999

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/grijtofoo.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gageqnqgk.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gprnqwwkx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhzmfwci.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gashktqfv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxnucyjp.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/goecpfmwf.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gscuhzmpy.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gddxeuryk.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwbkbcoj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyshsryi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsdtpesh.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gycyxholr.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/geupyusuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gkguournd.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gonvvhdhg.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcjauthwz.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhkyegsy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gsvguvawc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvnnymqp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gmolgbaes.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogalvyrj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqgrultj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/geqhygckw.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gydvvnnzs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gxnhqwehm.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gpeoygejn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvptjofce.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwghkyrku.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/giagjepsb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoslfomq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpyqufab.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/guvmkapnq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gygjfiufd.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmuoruqec.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyumcouye.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchxbttnx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjijxlrwc.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gtdsexrsa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntvgsbld.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlyhqijz.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmlyzbhw.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkpbzoia.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gfphhqreo.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrddiulu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcwvxbmg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqqpokanp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gshpdwzzi.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gfqjlixpd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gpurdsrok.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghujjyeeg.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gwcgmetxg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gaoyjumer.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpbirdly.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgvgzzcj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcqqlmwoa.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvrydsuz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gubfmkasa.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnjcaemk.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtnycszm.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gganzjyvn.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdypkgtk.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/grfjwexfk.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsrofsiev.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gkzzvchka.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gymfkenzd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwzmgpnv.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgpqwvyq.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjkduwuis.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gcnwpiyoi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwtiskrp.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/glbnpptpd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrdqhezm.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwwgeukih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gsofpibmt.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbxerxhv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grglaucgl.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gzghqmdls.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqxjipi.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/guccplnlo.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gvepcjayd.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjnroxit.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gurcqdcmp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gesrhcbqw.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlcofbsl.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtezqxgcv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gufbzikjm.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcrayrgy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswkydagk.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzlopola.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyaxysls.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/glvsfrdoi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggominohm.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghojnswdz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrvhxqe.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/ghdzvbzdg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynpofimy.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gadxpyapw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvlaaxcaf.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqxfdwi.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxqhvdoi.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gtewpncff.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlnunxmi.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqocrufyw.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxuysoxma.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxxzpiyz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgmyzvbh.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ganytzjid.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gffveryux.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhuqsged.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtahnvldt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdcrcuio.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gekurjgrq.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqwoppql.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqpkzwar.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gainmgwzt.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhknzvqx.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpotmtyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gmkhcbjwj.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyxkqsrr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcligipo.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbjwowens.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitepyjqk.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gaicscvqv.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsejoikxx.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gczxjjnny.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkmfccmdj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/glnhbeptn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gmloafqfy.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrtbbcnn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvzcskuxm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqotdbkly.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrpexmuw.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gmeamzbvw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiucjzay.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/ggeaelxoq.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsprwocm.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokbagxhf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/ggcftfrlh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/ghocygfvw.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpbkjdrjy.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gegeuweeu.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gdadodpoy.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvfxwrqw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnadmoapc.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnvawihr.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/glugnqozp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzvjmgiq.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/glissjwjg.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gissoyzqw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkrgewnd.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdqorynyo.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gezbzlkfw.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gwrevmupu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gezhfrwkx.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbbjupzq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvmvudgz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczhuneur.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkutidvec.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gdvypejpg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglhnzsih.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncgplqub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gglooqmay.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gnevxkqyx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbuxxxjc.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpvtdhud.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvmaqyqm.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gqpmrmpnw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gzzdsbnrl.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxrbdkfb.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtvskpbv.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfqwdowm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvujhjcm.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzkpurpm.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpvyzsvu.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuhkkcia.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloafsqmf.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkirbeys.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gkrwrelpb.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaagdqmb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gvjlwucfh.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuueqmmf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/guaivkbai.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gnmaurwos.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/geldsxcfn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjvwbqadc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkgwaula.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhagzgho.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gtvszptnp.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gywffsfkb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gvxshdynl.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gsxtebvng.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gzmvxzyua.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gwuzsvovr.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/grivermpe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfgvpxtq.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gadmxaehn.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkykelgp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyxjykmi.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxccgscd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gxgdoovoj.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gghknifat.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmjoadwh.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gykfdfobh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhznuwns.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/guhtrsucz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gchvpbnuc.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gxluetstb.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gvynkjywk.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykdtjemo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwuxhgifv.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyoefyxes.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvueuloyx.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtibxzuad.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwsiqqbp.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjudsdfd.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyteatet.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ganwgjsmj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzibwdr.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gnyyykctf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfuxlipq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gwhztabgu.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/guivjfnin.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/geqmjtuin.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxuvypay.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtwekngv.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/giuooonhn.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gntiyhpmp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxexwbzd.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghxxduzzy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gudckxrnt.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvplvkqkl.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gztdsowrk.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glysxveeh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gugruylae.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gszillgrp.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmuszndlp.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjzxgodp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gewzmodeq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gornujrnm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gphxwkgns.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gephjlcwb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaalpuyuh.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gqmgqbyrm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/guryiyrjv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqdqmmir.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdztwnum.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqrydoox.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gzhtyqcft.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzzmtvcx.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gocagcrxe.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjerzfxgo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/geezdrqeb.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmheejci.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/givijjtpj.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzwcwsvi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gpuakgscg.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjoyxfaj.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfdwamku.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gxbhjpzjv.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/guokilicl.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/giymgjrmp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/guemcfmfk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyghsyhol.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gekcpxodl.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gcgkedbos.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcafdwnp.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gsqyggnou.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gsrgawzuc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjsiqsyw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gtksgqxid.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gvylyvghd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gzmeqtkut.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgfvtfec.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gvbihjagy.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gackshfxt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/grugwygtv.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqvoauqp.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gasawqgrh.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwjcglgk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gwaabsjrr.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjizqlxdz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwnkdzl.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbmxwoxfu.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/grhhawszy.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdbwqcdjm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmultbgfc.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdbcnrzj.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gjzaqjvrf.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/glrphildy.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gcrythydf.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjptabun.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gvmkkfaup.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaxuhppi.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnkpzsdp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gbpndsjbx.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gewdbjltq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gncwuxgtr.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gerdkcfps.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnpmjrmj.sHtML


<!-- 参考信息 -->