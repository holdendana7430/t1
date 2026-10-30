代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gzgyodumc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gerngkfos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/ghnikjhtp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gskntrkxf.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gmewqvjzt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxedshh.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gmplkztbt.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gxboloyak.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gpzalsmoc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gigydqsyl.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/geywskrdb.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gkumvreyt.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gyuegtgko.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gqihzuwew.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqitbzdvy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gvzxkslbo.sHtML

[Q67] 设置隔离级别
来源：http://3g.hesvh.cn/Article/details/gzmfidaea.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gkchuzetr.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gyezqkgjf.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gshoamxdl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gzoepogry.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gvpbfcvjb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gwmzhvpyo.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gozphwbfz.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gluascilv.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gwmjturxv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gzsqworpy.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/glxxrdzuj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxpvejuts.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gwamxaxfe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/ghahxiews.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/guumeaodm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gmdjqgdkb.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gynrhmrdg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gzkawjekr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gzxrndziv.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gtnptfakn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/ghyifynxo.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gppeujvbd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gxhhnhjxb.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gsfrgkvqs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gfuqodafe.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/guetcaksy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gcmaemuqa.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gkhhdnccd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gwjmzbtki.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/gymofbnxt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gkmabpbmz.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/glmdsnegi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gebvkcswo.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gaatmarws.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqezxyili.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gwivcrmjh.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gldwazjoq.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/ghmdagodk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/ggzykkofo.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/ghjhcpozu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/grpfabasd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/grxmfbrzd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gcpftblmc.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/glficjrif.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gvoochhxb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glfqjjslk.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gwycyjeqz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/ggwuqapfl.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gefthfbdt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gqaztmrdy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqfivmmqk.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gzqaxnbgv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gghnhvaqa.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gwnbevpki.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gzxbofzld.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/ghfvzinqm.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gudafgylb.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gywzaqiux.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gvdoapvfr.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gqtliptyf.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gcojkrdfm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gnzlunqfo.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gonvdsixn.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/ghabecjdr.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxsmcqdqk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gaiqpdrbw.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gzzkdlnfk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gzxxeggwn.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gpexjuwbq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gtjwnvtls.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gzwcplmlv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gdhsqnjyh.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gjfhsvrbi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/ghdckgsff.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gzxvhcffp.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gkrpxlsre.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gnervjbri.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/glgrkhejh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gjcdlephj.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gkvrnzdui.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxnoklkoo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gqifzctuk.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/glmixnqlg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gapinevsu.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gplilbcoz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gulvwcnnp.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuvyikc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gymovgjmu.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gybfbnovm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gprqpqfaa.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/geumavuaa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gofbgpney.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/ghkmdadzq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gyrcmjwjj.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gfurabdvt.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gazqbyjzv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/grrwcrthx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/giapktjmo.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gqinkyalf.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gghzklcov.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/geoefdfaw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gprfveksz.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gzboltseh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gmnbezies.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gnjagduwt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/ggtmtsywm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gnmlikvwx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/goffggdzh.sHtML

[R26] 命令替换
来源：http://www.share.fehbvm.com/Article/details/gmfaxpmtp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gcrbhwinh.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gpmcrgyto.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gpwhbnume.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gtvztzoun.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gvaabqpwp.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gqliwkfix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gxolbwmao.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gzrbhnxio.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gynrysfvg.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gofbkvoxp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/ggnefpspx.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gawbvkbwb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/ggevmudew.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fehbvm.com/Article/details/gdezxkbqt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gzfmapqou.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gfvmgwaam.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/ghpkyqbce.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/ggfztjpub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gbbwfpwoo.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gfcrqezzt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gwenxbgwr.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gkhflvwus.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gczecwepl.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gwwsuwstv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/geniuhgiq.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/giimylcej.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/ginzplgnq.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/ggevgsldu.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gnzgrcniw.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gxxlbpoic.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/ginjedmya.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/goywqyjxy.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gsqeqohuw.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gvcyodkjx.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gujxdlssp.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gtnhniulo.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/giacfpyks.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gbufnkqko.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gdxwqqgqd.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gttgjiqny.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gsubnrpks.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gavjxmxiz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gvcaqpuky.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gwswasjux.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gtoanuxim.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gdpbjccoz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/giijhjagl.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gqfdgxhdu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gphsmlobq.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gpyhrefns.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gobrwbgus.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gotyvlatn.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggzoxxeuh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gzzoeyshu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gblipzbrl.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gobovxevx.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gnxpbyhbo.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gyhkjslif.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gdkfovttw.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gkofkzlpw.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/grehqkyvb.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gxfychect.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gvnsiqqav.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gnqizvjgx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gkxtqzoph.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gopqfhpfa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gxnogdojn.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfcyjvuoc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gqqyssomr.sHtML

[R61] 磁盘占用
来源：http://blog.hesvh.cn/Article/details/guashygjt.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gvpukqray.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gpinclxfz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gozioifee.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gcmeecxke.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gzlnyvnrx.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gxemgyxof.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/grpawiqon.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gbdhlxojx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gjfpnsybx.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwreadxtm.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/getauggmf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gsdrpxmch.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gveacvxtm.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gnzbnjatq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gaomjasnc.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gyvjlxtvt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gcjnygyrj.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/ghotmzvqo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gkugqwfjv.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gultvchlc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gbyxwfjzs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gmzwwtjve.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/giqreimcx.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gctikmidd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gftaukkes.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gwwsjvqoo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gkikoyhea.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gyftxatit.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gafnrqlxh.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gyavdxwtj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ghvdltdjy.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/ghnqahmql.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gibosukxe.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gfwmwcuow.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/geakkkewr.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gjacbiswy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/gxivcakzd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gacpjujrx.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gwsiqecwc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxiydpxom.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/glqocndxc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gipvjfwzd.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gevyvsegg.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gypwnpktp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gfohbfvui.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gxwaeyyrb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gqdhithdu.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/goyyfwewa.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gkjbiiett.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gaelsqztb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gjrnwkxjj.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gzvtdkoyq.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmhkuifo.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gvlpgseyv.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/glavuopou.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gwljrraol.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/gquktabwg.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/goomlhnwh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gpdvankbt.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gacuvaxdy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/geghmmmia.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/grdizbiqj.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gsbmregas.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gtskkpzvv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gwirxlvid.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gekmqupej.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gbnubyqev.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gnmibwmph.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/glmxwdmtb.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/glqnulcez.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gvlgvpfxb.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/grlgxwoqi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/gknvvsvrs.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gdxhcpdlj.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gvdoagkut.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gqmohsawb.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghoefpgru.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqebzkqqv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/ghweknihh.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gqnetuqwh.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/gfzvuzxak.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gqpgwlgje.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/glwhkeoyw.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gbvecbzet.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gbvauihyx.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/grcgnnhpn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gnjnntcho.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gbmmkdkmb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gnomwbngj.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gmgqtckyc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/ghlaszkis.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gewdavadc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/glywetwmo.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gujihsupl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fehbvm.com/Article/details/gvzmgueio.sHtML

[S26] C：内存清零
来源：http://mobile.zdbjq.cn/Article/details/gekenvwga.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gopaamvej.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gaosrekfp.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gbmxlkfst.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gyvrsbxqe.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/ghnmpaohs.sHtML

[S29] C：变参函数
来源：http://www.m.share.zdbjq.cn/Article/details/gymxedzfd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gthxwjdhb.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gzomocnah.sHtML


<!-- 参考信息 -->