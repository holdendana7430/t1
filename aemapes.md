代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjibjpkoa.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gujgadmyv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitqbgtpb.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsvhldbe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/giglpjzhi.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gjscsatvo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsjrzvgs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gxstevlaq.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gyngolptp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeuviqda.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gopbxjdbj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkuepqgx.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcdmrbql.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnochbte.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gpckmxgrc.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdfbwyez.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkylhhacv.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyaphzuh.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtosnfcpo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghprxylnf.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gowppcjbd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gxdetqvnu.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gbpxgzhhr.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxwylheee.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjyaqmbxe.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghynqizsc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gfecyhqnb.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gywupihfe.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfglxyre.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/ggffcicoq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnjndda.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gkogpicsp.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gskfkbjum.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/grbghfxms.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghxdnzdfz.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gbbdupndq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gmcklajtp.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwodmtun.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvxyntrl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqazmwyt.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gskszxchc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrizzttm.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwfbnwyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfzlarz.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gdkwdrdlv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gpojapfwt.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsuwrsal.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvyshgvx.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqimatpmo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbhubxhk.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmhcvhrz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrfkroli.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjnqfydq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giznozses.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckerookz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glimqnqmo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhtbylkj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvycfuamm.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpnblhza.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/grxbjhpto.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gvnoivpbn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqkgkpus.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gnztqtiyg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gxgdqfkkr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzibsqngh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdfpxbxc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqvzpnxyy.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdwbureo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gewtymptq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxftuluaf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvybaoaxl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdoggzage.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxkwgita.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmvhxfohe.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gnrtdhlyk.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gtdddmlcd.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gynafnnuq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbooipzui.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwblouln.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqjwtmzi.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gupoeduse.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gzdmszxol.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjposomeo.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzytbxzhm.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjmzgmtq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkbhzghj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcvszdgjn.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giuomfdgv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggiqozjzw.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdgxatfix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gehthkvuy.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gbouewhxm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginbntxnb.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/giotjmxea.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhvtqfbt.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxbefwyn.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ghkrybgfd.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcixzngzz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnmlhuvdb.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqymkbmc.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfxuevds.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gygvkbvxd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnvaqwlx.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvztdzvfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwslqqqjg.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gfmdvrrag.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkfcnco.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/guypuwaqk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gouhmxadz.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gaszipaje.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gjxdtovwc.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gvfvkokqf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gryigiloi.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/ggexxgmix.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmdedytif.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkekgaanp.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlblmlbp.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gknymipof.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoveffuz.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/guilxyfnv.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcixvjsdk.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gyfvlflsc.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieqkynbp.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gaujezelv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gllhdjypf.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gipbmoeju.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gozydetfx.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gwwpgggax.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdpwxdrk.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqlfjjjp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdheuhsxd.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/giffylsza.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuomigus.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/glecwoybp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjdxdvzn.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrjybvel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpjpoios.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfzxkcukh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmxdpxys.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/goizwxexd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzurlpbf.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/glrbkhfpe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpgineij.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerilonjv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gactvztjf.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwttcwlr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gprfvqgjl.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbnxzyita.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gcynujaid.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gryfnmsgh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gbeuakvcr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevwptuhe.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhdpopgl.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gwixfjoii.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/geodboiff.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrxiddvi.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gilqovukj.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbsozhoj.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gaddikysk.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gnvupimib.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcylmhanb.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/grghtikbj.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gszjlhtqi.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gubckpumy.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhurwgxc.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/grqidwctv.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glydhcshv.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gqiddseis.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gsiwiviit.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfppmxxdy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcwlrtwf.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxsceqyb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gljxjvtnm.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxfpbycq.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfheassj.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gihewjoxr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gyycufgck.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsjzfvszp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gliielfha.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpijkmh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvrgyqen.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnsglfey.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuwujzwy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gmmcnnwvu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaogsesrl.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giiwawzyh.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gywklgcqp.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyktjdps.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gtsweqhxl.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfocvzkgv.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/ginqzazfd.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpwryvvd.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gyvgkwxgn.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndoohesy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/glhcsvohe.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gohetfmnn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gscspgrqk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gduxhxoxf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/ggydzvlyu.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpqitfqs.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gebvqfbpv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gicbckzlf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/giukhegch.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gnryahrmr.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcnqncqw.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxvwirvj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glelxcvuu.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpitrvssy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gmbxpadux.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/grcukvvxb.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsnnpwtb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqkslivo.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/ghjvcqbsy.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gmwwivcgp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxktrayoz.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gywflxutl.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvcwlasx.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgqupoar.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcakipdrs.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gypofcywi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwryhkqoc.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmmymdgl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqbkaszyd.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjtjvpgk.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gablilkjx.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/glswgmejj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpndvuhyl.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpbxuizlw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/ghsctjocb.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkxnoynm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrtmmaus.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvsuvrvo.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqvcncpk.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/giihkklvi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/grwvkptzd.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/grwdfwtoy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzmcdbei.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagqxhjvl.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/goibkzudx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwakaltws.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gbouppzhf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbpkozre.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/getsneqpg.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gkufodtij.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/garmfxzjs.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpexxzncb.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/gomlqidns.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlesrkai.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdljtqfrp.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gwxpkkiud.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbxwlksw.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gklxlolcg.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfyzgads.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/ghlmmzyyx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvtzwhujq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtqligop.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtquejysi.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gamvnfblu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxguasjba.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gmqqyutxt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gkmsgfqvo.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzbchsd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlbejrji.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfycqtzgo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpvgyrzo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gxxrplzym.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwhqohka.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grhfrczgf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gydgsjpej.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhigorhb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gtrrngzpw.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gryygisat.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvjhabqe.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gvamupjaj.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubkkqbm.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqhstauq.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gogwbvkfb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltuznzri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gsybqicwo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnamcfqp.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/goemxpgwe.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseuemdjh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwodmeda.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqksrlcos.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gpwzjzuag.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdynvfgq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjkqhvtf.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjddrnebk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gwmaqsdij.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gplffrajt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gypsdzkbe.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/glalbpbdh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/ggzjzezsv.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxngxmdib.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gqqyqmiyw.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gtkyyoyyw.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gljxltgdo.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdcmvgwo.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gphrtglby.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdgvqbesi.sHtML


<!-- 参考信息 -->