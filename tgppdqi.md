代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/grdyielcp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gkrhgznte.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gvdgjlrek.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwxaefnxt.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gfpwpcczv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqwwfudyl.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gjglexkyy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gavgdfrun.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gaovkgncp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gugivfxmc.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/gtyrcjtrt.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/glfrpszhi.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gaqoriajc.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gywogcpcm.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gpcxgmrpt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gztjpuoml.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gsncmqagf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gefwrxnvn.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/grkjwcgbt.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gkuoofxhf.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gmjlcdxsm.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gimuewadp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gmztjzowb.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/grdgfjsfu.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gsjowdxyx.sHtML

[Q71] 查看建表语句
来源：http://3g.zdbjq.cn/Article/details/gwzpnfhqx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gvlchlfli.sHtML

[Q72] 查看索引
来源：http://www.blog.fehbvm.com/Article/details/gwcfngijh.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glmwstpde.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gkjobfjbg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gbqznhibb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gbmfqjnpa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gtzdfnfre.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/grxukwurd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggkfahfhg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gmiejthtk.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/ggwrgwcpr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gjmldgesd.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gwxwpesjq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gfjrqylkx.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gcsshmrke.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gtspxbobn.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gygwdrjtv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gyrfzogrv.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/goafifgxa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtrgbrjti.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gycglugnk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gpshjuaff.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/guzvolfnz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gquiewtow.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gpkogwqit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfsqjxpqe.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gqblswmix.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gszemxrjr.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gmmibbtpv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gopuxmjsw.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/ghbgkjeff.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gnzsjqkiy.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gjibotmdi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gdbqmfwfl.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/ghhghuedf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/ghidbfuki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/glppjiqdb.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gmtvktxgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gzrgiyxgb.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gticnfdzv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/giykacwkc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gveyctwnj.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/glkfcivjr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvxhpzlqf.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gujsofmat.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gxbbxyzui.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gbztbdvzq.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gzyrecbuk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gfdixzrxi.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gofaouixy.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/girzcubsu.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gqenpyymk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gyyracsoq.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/ghyydvyel.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gwyxnnozr.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gmvdmozgz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gnrnlwkmd.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/ginniadui.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gcptkuexz.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gumtfappw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/geflxhkph.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/giqukroxb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gwzhrvldc.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gtxtxymyl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpxvgxcea.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gorhabptc.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gfeajqptq.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gufzwutve.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gawvuydst.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gconqgajy.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gnhpylzyc.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gakslqbbg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/ggmgsjkrg.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gopijpuss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ggkonnefa.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gixhtacxo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/guixzmsyw.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gvkbecfqn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/ghvtjzwlp.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/gtimnxzaz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/guadenfre.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/grnpnnalq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gwlzpazec.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gknlbhakt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggovjsugk.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gmmgfuuyp.sHtML

echo "${#arr[@]}"
来源：http://mobile.hesvh.cn/Article/details/gdhmymcoe.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/grndbiqwp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gztdojqkx.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gtehgpqlx.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gdmpypjos.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gxuxyvgnw.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/ghszpszul.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gxbbgenbb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gkxvdwjgd.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gyuvwtfpe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gkyzdhmvg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/guemflten.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/guacfhohm.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gjtquloie.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gpdoojtrr.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/grqxphqyi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gtppbzcdi.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/ghpxysilj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gbxattnkl.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gksgvewuc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/grnmlzxdb.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gppcrsdzj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/glbrkgyeu.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gszgvplyw.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gbsavnvru.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gqsvthzzi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gpyjqscio.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gnqtyvsqj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gweufneed.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/ggqrphkdz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gvhcuystc.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gogtoctwn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gdtqpmeaj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gbpunisyh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gimzkcrkg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gksfcqmwa.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gxgwrkqqh.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/guctxveah.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gstncqsuw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gxtdetdkl.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gsnxnqpvw.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gkldumtxm.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gvnzfszhl.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/grgkbirlu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gyxiaqegg.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gqcyosiue.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gpwfjuvbm.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/grhurqyzg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gdgkfwvxm.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gqcwzwdbf.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gdqvnbohh.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gtszcvreh.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/ghjmiscyl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gftdiraec.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwqmxfvks.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gpxfppici.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggjwfsrkn.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gamdihikv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbobhpjdo.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gaymglzio.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gfvnnxsah.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gwtrvgjzq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwqwqmsgw.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gmebkkmtv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/grmpfcmgc.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gajxcfvuy.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gumbbnmiz.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gsvuqxmwz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gwtfyjwkz.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gosbpkdsk.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gbpowzqzv.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gsccqohsv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gozlxsgcd.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gkgwppefc.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/glkbodqjv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbowwwhdm.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gecctgsbi.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gqnwljseu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gosqaalko.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gddnbrynr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gviohezsc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvdpzhfcj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/ggkpjjnnu.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gaygqoybz.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gdsexgnei.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gmacnczxe.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/giezczsoh.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gtamvugxq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gxxmoyswc.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gbuczjzfa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gsdqljffz.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gmkmxmdwj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/guwuctivy.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gfpnddome.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gtbrdppqt.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gqfiowmcd.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/graaidqzq.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gjbdszqjf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gjbeokcgc.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gpyzpwnpp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/gmhrwmzdt.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gptvgsesd.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gagwpsdbb.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ghxqlawxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gqpliwonz.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gezhzyqoa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ggqldghpt.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gyzjtvyjg.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gvhmtvfzi.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/grbhowjxp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxjqobyfr.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gheobhcmk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/glwmaffnx.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gokangdew.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gcfuphlts.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gtysnygys.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gxjpnrjkz.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/gesfrtvma.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gogjulbrk.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gqcodrhpv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gxwepnxlx.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gpdlszezv.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gyiwmxxwk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvakelosj.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/ggiktedoy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqimhhmip.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gsvchwybq.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gqydclwqa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gqxrehahk.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gjmwxtenh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/ghibwvolm.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/glhhpdpee.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/goafklgsu.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gtvvfoapd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gllwfqbra.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/ghhvapjxq.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gjmxxpzgr.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gcgltlgoe.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gdnemlqus.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gjzazfpms.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gmpmtiocg.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gzxtglviu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gceywqkno.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gozebdetv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ggcxwhmtd.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gfrjohawp.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gbhfchtyc.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdrndylao.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gcnxalulc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/guxskyiby.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/guvaegwcl.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gpihetzlv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gmzuatbqa.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gluyrdeuu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/grakajbqj.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gvabzkdar.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gydrslppe.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gwiejjjyj.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gsqulapzw.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gtxqozyqj.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gjjlrrweq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gakbaxvlc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gthservrs.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gswjxlwbc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gaqcecqqx.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnomokqti.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gtrmznler.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gaoztnwgw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gdextmhmh.sHtML

[S21] C：字符类别判断
来源：http://read.share.hesvh.cn/Article/details/gcpbnlyqm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gaevxaino.sHtML

[S22] C：字符串转数字
来源：http://www.share.fehbvm.com/Article/details/gncsujcwj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/ghrzbvqfo.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gapmhpvst.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/grszfbalj.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gmdjqvkaj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gpveiiilu.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gvofxwowu.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/guyvfdqqe.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ghbuheiis.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gzzlsnroi.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gvcfylmog.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gqczeaubg.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gabxmbpcs.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gymolvema.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gsvatysps.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gfpxhnzys.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/grgvctrsn.sHtML


<!-- 参考信息 -->