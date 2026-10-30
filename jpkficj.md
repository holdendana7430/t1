代发 wailian999

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqnglewq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdefuwqmq.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasoxnhza.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gztresjsn.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsioxxxh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgsnmzyq.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gemhcjyvf.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgvuptzi.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gwvewwles.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdmzrzxt.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmgavuqcg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxctmytb.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwsfhnie.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/ggvzylutv.sHtML

[Q68] 保存点
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlqqkcpf.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmdqspbc.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwjqpzome.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gpnjoregt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gjgjyuvsu.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/giwelznun.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwndpnlb.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/ganqbhzpd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtoqmteh.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccvxvydb.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gonxjgfjd.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhqfzfkz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjapcrnhx.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gnfyzjznu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gnunchvlg.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzmqmhax.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gawxbnthe.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaszhnnj.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gupzqhzuf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gytbbsodl.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gajieiyao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/guhfwvpzg.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/ghxifbqnt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gabtfowqq.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gnjiuxcuo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfypeuhab.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gddczxkoz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gigbmtcwt.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghanukaqh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxjzdlfm.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gagjtzhjs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvfmtgjiy.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gqyndstme.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grhmunbva.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gphgcnbei.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuininiq.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhzqjofp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckxwpojh.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gywavpfdb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/guvskwiyf.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzcwnykaj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/glpvzkfwx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutvfpgvx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqksclvbd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grsehrazl.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gjnvfmepw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzyfebky.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gvuzntfgj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gylzpkzbq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gngkmkxhr.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/ghttufyxy.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcamoyoor.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gjooyoiah.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtombjai.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcfhkhpw.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/goovctvcf.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbnqemcg.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/goqrfqwit.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gafhcunag.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvwhyvtpu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwcekdgo.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gnemhxfmh.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzbljtbwk.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyxbgsnq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmblrdjov.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxmwfkfc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmovatyem.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gfrojgwvo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gtvxfpqdv.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitylsazo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgciekin.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrgropna.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxchtvxq.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/ggblsvapk.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gjckujrdv.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghevsghcm.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtepadmdk.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmsbbftp.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtbkrfbi.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdagity.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjmukmhm.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gwvywzcdj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkmdhrfc.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlmbhwua.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gjhqlbqjo.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdkrezmco.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gryrkbjzz.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuielsdz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqxzymd.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gsskghaip.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnmptrfyh.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gttegncfg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gdgkocwff.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/ghbxjuwkg.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmudgnufv.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/grvwcdyot.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfprmghsh.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gurhendom.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjnxdzsdb.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gonmugccg.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjrzxiogn.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gumfkcllz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gngtuagrt.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghntukpv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gauufmsln.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gukrnxrvx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrubjgbz.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkhfznid.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gackqrexg.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gibfhoylj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gkktiokft.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gaskenuzu.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gnlhmeaex.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbxgbujil.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgatluqh.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/glpchmunh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmwzhysgy.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkdtlaro.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgxwybar.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ghvudrlef.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmbmxbbu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwltfwd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdafazny.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gbmhewozw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmqexvwg.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqjswrnk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gebufgezt.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gipeuyood.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzmcbqmy.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnpkegmll.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdhivgjv.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqoirfdx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtevlqlps.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gbeitnktd.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gufejrpkg.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/ghatufwbu.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gcjhvwgme.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gxscwadcc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gpktissrf.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwdpkuwl.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcummeuo.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbfnnkkak.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfygjplwk.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gksymhudn.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gkebnwplv.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gtwasuxwb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gmkirwdow.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/grckoytli.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/ghejgbjyw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflcihrqi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ginbjjord.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/giwmsqbee.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyrtxcrh.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbnguuor.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmbvrrlh.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gunjhpwum.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxduqeitv.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjviqygn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqjiodyc.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsrqvrjo.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdrogswij.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gibrwrtmw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gpntervkz.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmolteyz.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glbvzeloh.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/glctgmrbc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gciayfvcr.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsunsxci.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqppzdhn.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfassmyi.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnwqyqtz.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfstxohrg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnyrvwim.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnyvyfuj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gaqwindxf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkqjlcgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/grxplrauq.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gpzxubdfo.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwshqbhe.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqsibpwn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gbzuelhke.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkrozgyz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/glqgaakox.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeedcraf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/godqwxuat.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/guvwiseac.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwcmqssm.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gbqdwakxw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaziugcaf.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyejpczlg.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gtgykjbdk.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwwgqbti.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzhypazuq.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goijdukcw.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gyyvbzfoq.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gqpalpulp.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/ggaobliqv.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpjxltpp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gasmafqtf.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkmkomlv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdpbnpzo.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoximhay.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gqgpgztmo.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gnhxubdcx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhyfwtap.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbfjvdlg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvdednnn.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfigajmr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gyuiraxvy.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gesegjhjg.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gynntllmr.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gryptxfwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giewymkmv.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsibulos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfjffpjxv.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlqhnxfl.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gztmrolbc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkywrtyu.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjtlzvpp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpubeysvh.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/geotnxheg.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgitvglm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gaulksjif.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjesvkqoz.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/goabgadrd.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govffpnoe.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqzepzim.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/ggbzwlmiw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqorjqrv.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwotoxkwn.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqicxgqjt.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqyhweqgz.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gdyrvrdlu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvguhzr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gkintuheb.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ginznkaiz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwbtsxsa.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtlckvada.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gryquwmwu.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gtqolsdvd.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/geaqljdyd.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumckbzfm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjntklzjl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqaibafv.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gdmbmqazn.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsfwccxde.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/grepyjsrc.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gyurcnnqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhxpfqir.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gqlgdbtyv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gylmdharo.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpputfmmc.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbsxqtws.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqneesiv.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garwonyev.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gljtaetrt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzptsothu.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gfvgwaqdq.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjxltjbt.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girquybun.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gddubpfjy.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpstockgc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gayhldbhe.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkblqshvm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gpzjjqyqh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gkfznxxjs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupulqbjk.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ggyjlldmi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gagvfuotx.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gkvhnfeis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gnqtlgddg.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvpkkpf.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gxxjavdfm.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcwxiegy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gxvursejt.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gljzdmxjx.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbtbkysh.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkoprohd.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gikdexary.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/grhvnmqlj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziagkibb.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezaushcg.sHtML

#ifndef X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gtdtavrye.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxdowifu.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gfaoessiu.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxafbwc.sHtML


<!-- 参考信息 -->