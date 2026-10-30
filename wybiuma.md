代发 wailian999

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvaebint.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpdogggr.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/goygcwsrb.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/ghffeocoe.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gufoxlpbm.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/gnwxkroei.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gimrplgcd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdeojhpl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzvsvway.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/grcqaneny.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gytstuczn.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gcigsjrzz.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gmwlgmjix.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gdogqagve.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqrahxvw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooouebnd.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnoffcir.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdqinvlm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/glprtonyn.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gacehcbae.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gumcyuxbj.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gdpnszxen.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnpmbldq.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ggollysof.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrxzoywy.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gezrwabji.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwthltelf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzvgpvgq.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwxvimbi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvvkjgmy.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxutgqyc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gybmidcwu.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/guxmwtgml.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gplnljxbh.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gplbeorcm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gfltewffa.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gnclomywv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gudhkbdix.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpvangye.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlgptimh.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwsxlfjh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glanndxei.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gerwevghy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glpvunicw.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gzsebtimo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbqsmxghc.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/ggugdsxwx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gqilzefoq.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwacgjcki.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekjmzslm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/ghgpqusae.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjdgoydr.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gxxctjatm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gjymjltxf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gdjmjvswc.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gapevorcj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gwljbovrx.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/ghzvnqlpg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gwajbsryx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvootewh.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gokibflzn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggohimbgt.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gnxewobsb.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgoqyecw.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gditlemjh.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gktgqrdbu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbpjsmwc.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gujloapig.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxglhluk.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/ghjjomeht.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gqphygpky.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gkhqbqyfz.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfgrjtlb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gouwsmfvz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchbltwav.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrxummxz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjzocqqj.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtunoddnc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ghjtmscml.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtzuandg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gkefjtiap.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gnabizhyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgfzhsnw.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gvxmhlmkj.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/grpsyrknv.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grpnovgum.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwltipwr.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gotjgyudu.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwtqhchj.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gekexbxdp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqmkbtsld.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gfaakgkzm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvwxseiir.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzovmuqo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvpfpvoge.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghrxyloax.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvponxnhc.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goosffbnn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfsazwrch.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/grsdrbvqt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gyovolsbb.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhbeixb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtadrqldk.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gipzrdswp.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghoedmyhd.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gvyabclbr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ginpoqdfp.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvvygnvx.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvusfyvm.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgeyaqsg.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gngmeansi.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwrhmdcl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcvdozhtw.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfepgrylx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkpenhqyn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsecheno.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtulqsrli.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaovpevco.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkexvgwzn.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gfbiuhuof.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gmceqlcfz.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/grjytowlj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmajetqpy.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmhyfqpps.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gokdvlxle.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqygheqdl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gyekxtnvg.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/giakrbaww.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goluhohpc.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynvjkdpn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqkmgqzmj.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ggrbcblfl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlfogcyh.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gakntmgfb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gznrtoqce.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gydakwvvd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graetmvnh.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbtzlvib.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimkkleiq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grxlblhsz.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gheutzwzt.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjveptgcq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gbziyifxe.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmmnuoke.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gsthdujum.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyybcbks.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gclhfjbzc.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/griiqqiml.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gtpymzoau.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhlmvihc.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gumcafmlp.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gekpaytmr.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gjvrlhrqg.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gcwccemjp.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gxgrldvyd.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwoodoxi.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcurmmm.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozxktllp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/geessumqf.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbqswmesu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/golrbohei.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gbfsbbprx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gffbkbznu.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufwkfwfe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gclcblviw.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/goxknuwva.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giswrcaqr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboyvclsx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkmtmbzr.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gkesrafcu.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxehzmwg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gslxzorvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gzildukmy.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyqctilq.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjronycvu.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwlukroz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxryanpx.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/goyjnzqya.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmyciqsp.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gueybqxly.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/guogxuems.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaefkupvd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylgdnqpn.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrfpmuyh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxydybcin.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/geriwoeim.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszjjhiyl.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlguwnug.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gxffjeidd.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/glrjajuyv.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gynufsfez.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqlpxppt.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gxcikxynp.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqvhjwsvu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gnvoghpuz.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgxekllv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeijgkpq.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ggirmaqad.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gayvtrsez.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsdhcgdj.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gouvypslb.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcpdpxtt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gcomcldcs.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdkllynn.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gilmuduuz.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/grkwhxjti.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/geejfihrx.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/grlezdvkn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gtpepkesf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbbagego.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gczyeivwe.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gshdtrlvq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdszflkl.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gzrvooval.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gisgwlubw.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsqttcyba.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/giffmmqgv.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnosbdqtd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gizanvkll.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjcxvwre.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gqznptwky.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwqcuycz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfkitftts.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsmilllh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmvnjtiss.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gyllfqezo.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljmgdbrm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvarzmn.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/glsmxqjqo.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbwoeatuh.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpqrtrbk.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfjklkj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsyvbgko.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhiakwwu.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/ggxlxnvfc.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gufcyvocg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gzcrkcgrp.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gcumcfkhr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoiehcjh.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsvjmfaw.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/glgoxalye.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gruffdgzy.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/glmuqanim.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccrvguef.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/grwsgzlqs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhbidkmk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlbmjnjw.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gscembjyg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdshbvin.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtjvghwd.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnafcffn.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/geexlotis.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekfrbyoa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/goxyirlii.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gfotvkkdu.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geunmymbx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkmjypwo.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcpttnsx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpxuanl.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwxokcrxa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuvkhqle.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglzngdnt.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/geatpfzuc.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gpjpmoupq.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavweebei.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbbqwqqbn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gjhissvbf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejlulssj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgqmwuxx.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqckuoak.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gilamnxyk.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/grvelembo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/guutxcbel.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/ghwuezqsl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gooiemojh.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gplfztgbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gwtjzjewf.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gylzphrws.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwdovsqj.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskotdgof.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwruqlld.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/ggjnkerbu.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gewkmeyeg.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecvqrrgq.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwzlxknye.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqxfkkbu.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtxtaogz.sHtML

[S28] C：静态变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbvucmgf.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/grasombeh.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gpshvwful.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gteticmij.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxmdntqw.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gcgmmnxqh.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzcxqvwz.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/greryguhl.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/grqidxxzq.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqhgqgpu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozgowzdd.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkcvjqvg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gmumalcmh.sHtML


<!-- 参考信息 -->