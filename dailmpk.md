代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelycycyk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvoemizh.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gozpstifi.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gxakdpvav.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlxrwjbi.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgldcgzb.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkveeuniy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/giqagjchh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gicmspdaj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkramnud.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/giuqzfngq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgodkfhh.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gasgxdzet.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/geskmklnz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqkdekie.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhqdakin.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/goowxztui.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gfxgzjmtd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwurbzaq.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gaszylnwv.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpsmdake.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gxtzgpbom.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbjmmllz.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgyubkib.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gkwuiopwh.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gktrpzkgb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxboalhe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gifixsagg.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gvekrcolr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gchpkxuqr.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbbonyld.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcfjzfwc.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gdawkqudi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqedhmyio.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gfwikgqik.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/ginceykvx.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gsbtdmnkj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gblhortlf.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gydrwhwzb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gewxwxbad.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gjkeryohe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpntfswir.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaexdaxfz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gachmpbky.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoomcxba.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gluutnhid.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gyyxnwdsu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvgixzxp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgogfqfa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gyybukxzm.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyojscbw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiaqxicd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevipqnhr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gstpzkedy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gihqwnqtt.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghhwfwhue.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmohwbxx.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlkebixg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxldtmcfy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gyyjctqny.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlzcagns.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbsjnrjoo.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/graklibxm.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/glyaywtkc.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwvwveou.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhruzycz.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gwvtrezmw.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/geedzhvoe.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvfbnrpb.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gswezglrs.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/golpjufqv.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gidgaiatd.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gtztqmqjo.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzteknoj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/ginefjfdc.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvojbsahl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjjyjpvf.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gyciegizs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpowvyui.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzochusbq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdefflgxf.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gzagguyln.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gojowaduc.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/greqwigay.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gkryvgwfg.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmczsrpv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpszzkgr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gigtvoqmq.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohifrtfe.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gpuccqpah.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gryminmzw.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gsksocujw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/glgazvywg.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/ggfntanqd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnransvdv.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyslzxnlo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdrpmygk.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmalhwwka.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geabbnxfp.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gazzwxswj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwynpzhdg.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/govqhwpgj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjcodrzk.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/guvddjyqh.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtvlphqmz.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gthdjzkfc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafqbxhtv.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnlmaedpn.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gxjlisbyz.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbscfolb.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluzsdkdl.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gltkwxeeg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsuuzvucl.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gblebwoua.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzusgud.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gbckpozne.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnrtbitys.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpekgalti.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gykfmkvot.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gudrykjwj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpuoxtjm.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gftodkvtf.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyolqnyg.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gliamuocv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gajaohbiq.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ghkknahqm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsehauhb.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghromcpqb.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjhiddpd.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gywpnlvay.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gplaqmwki.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gezhxozab.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzdlslxx.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gwlpmznpp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gofrwakfh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gaggqffun.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gfuvnqpiv.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeurmjsz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gyatsiiil.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjsftuse.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwxljettb.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gprdrnahj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczgnxkjz.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/ganxhtwed.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvkbqyqb.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gcmdxbujz.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gmmqcjnld.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gcqqffcez.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwqwwvaca.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gyhrnqbqe.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxarsraue.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjqyvrmti.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrhmwhxu.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoogujah.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gbemvmoyw.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gccjuqyer.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gloeiwrul.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gfgvlazwl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/grnaymdtu.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxotswif.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybmmqyge.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcyowvmq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjctacgun.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gljtibxxq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeogbpyf.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/glpnckrzn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggkzbietj.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gsulqozbp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmdjaahm.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gsrqogugw.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvytuwsj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gioldrtph.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjzbbzba.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grhjuxlkx.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gknmpgter.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbznfrix.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikmlxhgv.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/geekjkqdy.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysaxwohe.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gxxgzinre.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlvjaduw.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gglfrxtnj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/goctppcpi.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gsssbdrng.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssgplvbx.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gbigsalgc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gubbjwxst.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtympejeo.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpaiifid.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvqhdnnjj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldsavwns.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpucfphqh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gaydyxggw.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnujrhty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeqsovfm.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevykoujl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/geuosvfnf.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gjcgzaeug.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjoqkjju.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfljntnpg.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnuigjpc.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gmizmfyyo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzantgisp.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gxaaprtab.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmymklepn.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gawcjfhrj.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gviybqmac.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guimkwqan.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gafgizvqk.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkctsqae.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gysrfiixg.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/ghhriyxxf.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gvbiznhrc.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/grtaatabp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/glxqzklmu.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqucqqwlz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwozwsom.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gggrzkkww.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gomnlkdii.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gxsdxvwfq.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gnrvswklj.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/glwbexxfb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gniazxyoo.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gajanbnuy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grrpoznfr.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gfrsadsnw.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfrlkcdrl.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjigvvqft.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdwzdisc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/glzmhdxrx.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtcfbvpe.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gohjgcisq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdgubexj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmyyuesu.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggzokoiil.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/grncehxof.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gucijefhd.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwytxrjn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/golrecump.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gdbxvfegp.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsriodrf.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhiizhog.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gppisiddf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpknqnoa.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gpuffteaj.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawyxyrq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gfewxehao.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gatpuvrer.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/grkmbvqsu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkfbehlp.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxszloihy.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxiyzwb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcejbqlse.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopdtxufl.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/glbtosnwg.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzrqmfjw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gebzehial.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskhiuded.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhizlvwa.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/glqkpyxwe.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/geeiugllb.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemuqmszv.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjtcsjex.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gbhczawbi.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gmvnnekxg.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfkwhieiz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gepcnzfxn.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqolcjaby.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/glvmcgkzi.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gywhzbtxc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gntnbkeld.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gyiwpibhn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gmukeojon.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/geustwkeu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gohvssefs.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gcycanmdr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gycvgbgvx.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gepgamdec.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggayngmzw.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcmmklro.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glottnnmz.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/givenhdmh.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgiolmzx.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/glbpreopt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijicrtba.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gyfjyremz.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzrqevlj.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnondiusg.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtpcbbmo.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gtefuqwxj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwscbfyhq.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gaukqmgih.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gprpsanux.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gwvljikwz.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxfmjccu.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gixmnnvae.sHtML

#include <iostream>
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfmbzpwz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goftzuwlb.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwqqngsjn.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gohfuvkov.sHtML


<!-- 参考信息 -->