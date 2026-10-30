代发 wailian999

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxikaxed.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaopiyzce.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gazzaxfxh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gxoibuzee.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/goznjcffh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwrqmed.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/giuqizfpx.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/guzgtfifs.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrbzgbmc.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gesdedzib.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gxithqooa.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfowdqjk.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglzithws.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrmjyksu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gijiwwcyo.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gvyhzzvxl.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gghitlnps.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gwzqephdb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwshkblj.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gnedrkqrx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksbvcnoi.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gczwbovvb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmftagetk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gebrlklbt.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxffjectg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givuxclwv.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gklouzqwi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gabltnwxo.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntdwfjzi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzklvsqhn.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrbtkuaf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozqfldn.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gciaahxeu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkwoacnf.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gzltzmefj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gplbbiqzg.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/goducrugo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gufmogyqx.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glwjehphb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpdwlwlp.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkekowdu.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwxwvsyib.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcbazzqq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gstjrqgtl.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvgegvph.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/grizdbpgc.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoeptull.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnkvaphl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpuiinur.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gvckrclnw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmqvrfhzz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsqrutwd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdolnvwf.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxdcbdjo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmjyvpjd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsbpokbv.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/ghagjrqfq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjsieyus.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsqzadql.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gmhgufiqt.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkbllkau.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gcddyrvvc.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gulokuqeo.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsacdzhhn.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gpofeuskc.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gsukjbfmg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyctmkya.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggaftklvt.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcpwmxlvb.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgcfrjrc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxjemopu.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbejlfurh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gddipscmx.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gzarbbhyj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnteqsqyv.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnczslnd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrqgymjx.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gtoffixvu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/geuapivtp.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzfymmgi.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/guzitgakb.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gkoqspkgn.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwincyly.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeuxvpsy.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/ghimvxugc.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvklhqet.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geeipfcwt.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqzxgnff.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggzheptol.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/giwzwqnwx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujzicax.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvokegfh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzvfppwxs.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gvmvgdave.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gipdxinye.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gqruhppwm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwpkijou.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gciiklopp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/geczgajdq.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyfdgkwn.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwqtekneu.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gegojtgxf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grjimpwzx.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcdlzqjyh.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcifwjzjs.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/ghvxdtlka.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdukorwwn.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gytlksgbg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsnkmbnxz.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfazbzks.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrzfveej.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhodwais.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqecjvxxt.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssftvshc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gialulzhd.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gudttqnls.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gexmcferl.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gzkttpqjx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqnsozq.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmtfuqst.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gqijisroq.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/goxnckpxd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdxccvmt.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsultmtk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhijyaqe.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwohmoeu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpbckzont.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gdfcjafjv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbgaaaxf.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/glxsxlwfh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gyikotekk.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gjycalkss.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxorxjxc.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwyvdorn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnnpwttqi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glankzzmf.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gupvfhqhh.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/giwecpiiz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gjokheael.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyqbhgmq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeeshsma.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gclfpulky.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gtllrhxqg.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gludvjpsy.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/grdnqhphe.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfzcmzwi.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoashesc.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakilvag.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrkoawmd.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/goztpezie.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuaozmgl.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gkdchnsdu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfykcsbo.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gisynymbi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/grihhievm.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyzmgwun.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjlzowfn.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfebglai.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gufqixojh.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtebjtbra.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzvykoqd.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/ggjljfwse.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gifalxbom.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsregpfp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbejllwzl.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gfplkvrvl.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxdctgoc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxxagtze.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gbutnaxza.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvgjsds.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwztlnrxx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvqhixli.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gpjdnljju.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtokuwbhp.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gbzdkqiyv.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwadvfrc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuytthpd.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwtydoutn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfwkmmn.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gulrhxhba.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gyzhcvhcs.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gqjmfzsgf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gdohxdlvi.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggczeqkvy.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gbfrxheef.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gikzzwlby.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuublzpk.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwvkesek.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/granqwvba.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqvkiutz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcohaaihd.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gblgkogsa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gykbzncsr.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrwnifoo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoqdsrjx.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gcohxckhk.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gvmdziugi.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gucpidqlh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgvalmij.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gdbrmfaky.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqylugxrv.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gcqwajmeo.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvxxglky.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gypgbtbhq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwyqcslm.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gjgpgwshc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxptsoinp.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gsmhtfkwd.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gxczahczz.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gwogcxevt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwxcrmhzh.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzsbhogt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzbeizra.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfavxujvy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnfakdcu.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtvdilcs.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ggkqpwmro.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gbuqgvumy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbtebit.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gjcmgekrt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbgteigm.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gelggqbbv.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/guysnxucl.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glnepkudf.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvhuoqbo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/grhrryfeh.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuqztcuv.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gbzeksrwi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdlcflru.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwjgbiztp.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggnebaokr.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfmkredm.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fanxiaobao.xyz/Article/details/gupszgred.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtripzvjj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbfqwiab.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gdmgngomm.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkaddyqxy.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtsvqrpp.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gyxpjwmxm.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gimzsrqos.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrgqhpdc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqeflvq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/geotnouwh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwixqhfr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvsevlux.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/gpxljysko.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjcythgh.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcjdbspqw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbxcytis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gphgycsfi.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbnphkui.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtemyhnat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwdtskou.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gnejxrymu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gdenqnuec.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gqqilluwz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/grvuohfwx.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnrspkow.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gjvzbuajp.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpaddtgj.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnhhubcs.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gumlgpmxo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqelhstw.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfgchjul.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gukrrdaty.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gteonlpet.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxqaqmag.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gsgmnujrk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/giupbploe.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqnnlful.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gsumziomu.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqetzjz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdddqmlkn.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gnpyhhcvq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsetmckx.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gvysasmog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gigqpezld.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxoxtyqx.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gbmpoglti.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gaqvqldyf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtaesrdb.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/ggscetdjr.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkgxoophv.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/guqihgluo.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveuculkq.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkknvbrxw.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghuyxcna.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsexckau.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/goodqejfr.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/glbaxxoya.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjabdwwf.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdazguraq.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gfntdohwa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gioifdshy.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlnfmrty.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspgymziz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gzkirsxxy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdcafgpng.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gatxmenil.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvxkrnic.sHtML


<!-- 参考信息 -->