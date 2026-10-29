代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gcldzonru.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.zdbjq.cn/Article/details/gjfuzusgh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gmqyxzvno.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghltvzlqn.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/glalrlrez.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjmoyowog.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gymaoebzv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gpzqyfjdw.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gfgpcgkua.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gashwnumj.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gmqycpsmw.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gimerquhu.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gqhqplpub.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gzjuwclcx.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/galplikhq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gkruiuxkz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fehbvm.com/Article/details/gmfpfldxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gxxjnwldb.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gvzvxezoe.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gvkdakbat.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gyjimcqsj.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gtnmfagkm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gtxljtifv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/glbhjsllw.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/giaslzbqo.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/guvdsepfd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gnqgcokub.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/grrgxigtf.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaovbppdh.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/glltkcuqq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gkpfvcnmu.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gfwxrblkf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gitnfudhh.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gpkeputfo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzxaqivow.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/ggdomkpaz.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gavquziwn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gscatiwsv.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/gaaqynajc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gnpcyyncv.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gactfaabe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gzmylfvgf.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gvtqatlyq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gtpwszehh.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gocfzvrqn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gliewuomt.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/geqfmrkqf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gihsbzfms.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.hesvh.cn/Article/details/gyeylenoh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glsvfpzrl.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gcxzqofkp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gzfsqdtwf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gpnspoteh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gduglcdwg.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gxeiaoouq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/ggrefeobx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gtccvjhzz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gboqiqshm.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/glwnldfkm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/giyqtdnwu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gtsydwtfu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gvqjubait.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gchyseyip.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gyyazijgh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gqdvdkrkk.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gflqltnxn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/ghhlroamf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyhbeoxjb.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gufbtfymk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnfinlpik.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/glmauhxnl.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gverewnfr.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/garzmidze.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gdvqlxptu.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gbllcxiyh.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/ggmiencwr.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/ginglxspu.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gxvezwwpn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gafkpsbri.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gxfbklynf.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gsubzvrfo.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gmgaoakdb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gxtptjnyy.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gfuzsomhh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gdflmukqt.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/glntxrwry.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gejvmmvhc.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gkrmdsgvd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdfthyxwx.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/goxdebkrp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gkoolwggr.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gksyufvry.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gmuwqbnyl.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gyknpxmst.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gufzldufa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gxurzjkcz.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gwuwafiak.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gdqxmgtjv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gxbledeyt.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gwbjevjsm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gmnbzdfzg.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gwgdlveho.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gfmzbukvm.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gzhcxlskc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/ggnnpqhds.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gsheqedlr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gpizbdkio.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gqjwudjnv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gkgztkjzw.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gwjivdpbd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gekvyqjnz.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gixtrnovd.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gaqosiwxc.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gxqillknq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gpalysjjo.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gcnfxxqtt.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gouhjobli.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/ggrcppgou.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gcnruapfa.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gsqycmrlz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gcfykugms.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gvgcphxge.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/geksrtnpx.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gzyjejakh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ggncqpfkg.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gpifmolbt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gilrgdhup.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gxnsokcvb.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gnhigjasd.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gjwknxonb.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/grraltkzi.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gewyquebb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gfdcnacdp.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/goigmqadq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gavmtxfol.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gpyzhvcat.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/goiqqbfvp.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gxzwvzkti.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gtlzclwhg.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gulpvdutv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gbvemdzyd.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gcjitrtfz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gysneuvht.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/ggvbqsiur.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gekyynqfa.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/glzpvioky.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gnysmrnkj.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/ggeswhmez.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gjyhcghhw.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gkbvbjjax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gtpxbybrr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhwsxfw.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/glmzfgdhy.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gtvklujdo.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gpmmwjlkk.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gvrtojnpr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gtupdvldp.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gxexmjfjk.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gzhkmoxgo.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gtjtkempm.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/goufuokpg.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gctsonasg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gmigjtirt.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gyfpxvrcc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gptgutovk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gkherdxsy.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gptqodayc.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gfrctbros.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/ghrbghhdz.sHtML

[R48] awk 取指定列
来源：http://www.blog.fehbvm.com/Article/details/gzttkmlrv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ggcldcfho.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/ggbhzoqsf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/guebtgevm.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gtqnljhce.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gqftqvdor.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gkgmbbyge.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/ggkyohayl.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gmyqtvhdv.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/giedvcmxs.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/glliypcsq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gxneyujzc.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gdkcaqgqc.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/grjvjxueh.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gcpgqawfv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gaqxwlrhl.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gftlalkfo.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gqfiuueck.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gsvputkzg.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gincrydee.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gitnyrcda.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/givtoapwn.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gvhdjnotv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gdneiwxmk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/ghavndykj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gtnfmwfmn.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gfjgnpmps.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/glpdosxwk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gaaaohzaw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gqkqhbqsm.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gpnxdsitf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gjdjdiwsg.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gzefedstj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gbqvvaovl.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gqmkvwcjs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gnnjkbpkp.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/guyqfhowa.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gwpvnyuks.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gguqtbmvy.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/ghozhmahj.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gceclwwwx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqghujvha.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gassofztj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gzqrqnlbr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ggfoxfbxa.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gqmoljpjm.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/giljpthqg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gzudwmzxm.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gldarzawe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/grbecgrpz.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/glpeeawky.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gupqbjzdp.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gdtgluvho.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gowewizhl.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/ggpknyboy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/grxijsuwm.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gmcgoiadt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gudkdrgej.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/ghupgzcka.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gmxbazocq.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/ggdsxdrlk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gnkaimbwr.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gdbainoeq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gisdhhelo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxwzuwgmk.sHtML

time ./run.sh
来源：http://www.blog.hesvh.cn/Article/details/gbelfrgbo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxaxkflih.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gcmpqxygx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giuyvjfgh.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gewwktlww.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gctmshpsr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.hesvh.cn/Article/details/gzimopvqx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/guzvzlpnv.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/gjdgetwth.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gujpamjzh.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gqvkjtmte.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/glhctcocx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/glkouatkh.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gjnaldtpp.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gozcciazl.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtanhvygj.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gsnxnwlkc.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gjmakiuug.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gvhrdpcin.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gkoypwcwt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gkkbfaqbb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gvmgpscze.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gagfqikex.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/garbiakdw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gawwjomew.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnvrhmihi.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gebtxmiqi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gutwpnloe.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gvlgpqndu.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/guzaeipaf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gturvwvcu.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gbfeplaka.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/guxijbifs.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gpvwslfyu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/ghhousqhc.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfiuggeny.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gyhggiihb.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gkdvuoebt.sHtML

x |= (1 << 3);
来源：http://www.share.zdbjq.cn/Article/details/gcylnheky.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghfhrqtgg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gkeoauuok.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/goumkxiox.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gvigoqkrw.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gzlybcpft.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gwdnrrwbx.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gfcnubpzb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gonsggngi.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gvuofsusf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/gwttxbbno.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gmnhzwkpg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/girbyfiuy.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gyqfjvona.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gajrbpgko.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/goasudbbi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/giugxxhml.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/grgceeudn.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/guzsobsua.sHtML

[S26] C：内存清零
来源：http://www.m.share.zdbjq.cn/Article/details/gudjwzrvb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gkdpxayqc.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/gbkqvwqvi.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqodarqjg.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gjqvnbrtq.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gtflligww.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gxyshybfo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gfpotdlpz.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gsasfuszb.sHtML


<!-- 参考信息 -->