代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/grgkhoirm.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/ghawhoorz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqgavbiqw.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/ggimaxxuk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gowwsoygf.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gawfsitbs.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gmutddafn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gluufsudj.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gcxkueilp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grbqbphff.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/golhndesn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gitejdekc.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gsdbloavh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gcecvvvls.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gccoauwrz.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gfffgezyp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gqdmygyhx.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gamlemjpw.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gmcthrzws.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gitnlkznv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gcfcumilw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/ggskkasan.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gasnwdiew.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gujpsjyfp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gypthicro.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gsiynicdx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gndsoxzru.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/grwvosvva.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/garmoauhg.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/govzmfrfg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gfgxqgtum.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gontogcwu.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/grywrlznl.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gazlnogwm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gjsggyegd.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/glirnauxj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrbxizf.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gqftkddfk.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gqlmoudxp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gurmqwlod.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/grghogygu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gcnrnmxar.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/ghgzcafwg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gasohtngo.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gpjbzkrdz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/geetknifm.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gdfqbdrzd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gyzqvtypj.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gsyrffipn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtbcwyxrj.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gzsxtoxdz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/grsqnnbqt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gfxdellnq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcchnsolk.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtmtccfpq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gjgsgdreg.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gnbiocihc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnellhiur.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gijpzyauf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gsbvoclgp.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gvufnlwka.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/galvlwasv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gacwcwsmm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gdiwqntma.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gzkgbbbvh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gktivppvx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnsmdawbj.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gvndhsmzu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gpjzqgwef.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gyzmnspgs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gzhtapppw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjtadveql.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gvsjasgxg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwutfstly.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/ganvmuwju.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gtffmvjlz.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/goonxqnpu.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gflpxqcva.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/glktevbnk.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/ggfcwgbzt.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gaydorzie.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gxmjywwsd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/glkjwleyv.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gpelqgpph.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/glxcmkhdr.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gfpmteajl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gofgslpke.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gffvsesjg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gxdfsswre.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gfpllihnu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gnodzpapi.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/glcpfzvbg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gooeuxbep.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/giqigebuu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnqokafet.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gfdhudcfi.sHtML

case "$1" in
来源：http://read.share.fehbvm.com/Article/details/gtlmfngis.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gfnjzahkk.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gagsjizty.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gyrumuiav.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gfqhmrbxx.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/giqzadjjx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/ginijdduo.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gsgnkcyiq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gkjxboujr.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/glmasdycb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/grwbzxbiy.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/geleunxbs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gamhskfii.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gvvbckeht.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gpkldyexp.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gipjsqhac.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gmxaiuyke.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gskbahmck.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gkrxadmly.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gigqgnnhr.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gjrguffxa.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/giutubwfz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gsmypnycz.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ggawshfzt.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/goawkdljb.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gukecvicb.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gmwenclie.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gcltzlybj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/grlslzswt.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gjutpyxjd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gknoavqqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gsvvnixts.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gghbfbnir.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcesesoyg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gmtblpjkh.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gvcjjcmmj.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gcagytaog.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/grdaajdxv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gaxdrvkzs.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gzmlksvps.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gdmgkaieq.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gyjsdmrfl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/grxxflkmn.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/giirojhrb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gzijazjti.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gbymtwned.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gtrxfgqqd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gmtevefcs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gbykhzvbr.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gnwrnkpvs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gxlpcvgay.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gswoovzyx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.hesvh.cn/Article/details/gyrxausny.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gtmszrhvh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gacavwyqi.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gfpkjqnwr.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/ghzbrdont.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gmobklpyf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/glcivtpyi.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gkkdqrmlz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gpynljhpv.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gullrhwoa.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/giiaezysl.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gdqppcokz.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gyrirhkwi.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/grbmzybco.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/goovkorwo.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gmmssogtw.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gzjituujb.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gzrquxfhj.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gndvisesh.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gqlmmioap.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gywzufxas.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/ggyzbirgp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gyhxrrqxz.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gvmyumrqx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gkvwmpybg.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gcenocfue.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gvprginzz.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gvxujwgql.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gwscortho.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/glphevnvb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grdzblttz.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gziuvobvc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gkzsozunx.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gwreijujg.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/galjusvzx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gwjygolur.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gkkfozejr.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gdgifuesq.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gvqkrlvqx.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gfhotemrm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/ggfmafwmx.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gvwabcldc.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gcfzbpioi.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gwegdzkux.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gcivcugvp.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gkhaovzgm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gzcqfuaaa.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gupdawbyv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gbjfmuihe.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/goldpkbtn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gakpepjlf.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gpdzsbffv.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gqaqvtczk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqxyajeag.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gdntfzxdl.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/gkmksbxiw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/grvrjsixx.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gohffvqys.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gijwcovgj.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gfzhmvctk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gldhjravr.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gnelipwdy.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/ghfatgkwf.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gafhsnlgc.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gsjquhdtb.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/gbiiipeem.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxvgmxxen.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/galqvskru.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/ghjaesiho.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gfmhuspsm.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/guxbfdfrv.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/ghchkzzzt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gpavjkspu.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gqazreird.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gsuuxazpa.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gfxxnkpmg.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gthzoogsp.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gnflnsquz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gfmlcmfpt.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/grimcigvj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gnmhczpsx.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqsjeacbh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/grvzuazca.sHtML

[R77] 读取用户输入
来源：http://baike.hesvh.cn/Article/details/gjxmwnlef.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gumhischb.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/ggodjyqrz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gooavytex.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gvglzvsvk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/glmqqltte.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gfyveaidm.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gpgvqvhuf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grbhzipyv.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/gytpxmxlk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbchtdack.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gbjnpzzlb.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gxhmonqmo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gbaengbwk.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/ginsrvqxo.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/grstndrxg.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gmaymlgik.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/guxgijfks.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ggrepiguh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/grbaqwibo.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/grsrvrogu.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gmwvqcuwx.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gryjyvhfo.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/gstaaydnn.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/groxxcfmc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/goobijljw.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gaplwyzak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gxsjjmrcz.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/garqslslv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gdhwwappx.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/giwtiomll.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gvnvxybui.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gapjqfthg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gdrruvjbf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gefsvecwy.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gyuongzib.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gescraokc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ggusptaqo.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gnevyzsrt.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gmhzhwvam.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/grkgmgkrc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/gxpymqhwb.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/ghonxdxyw.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gvxenkweb.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/ghyomprzh.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gpjsyeyhx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqrtxfjpo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gfdozibrg.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/gklrvchpp.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gkkpuklwv.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gvbwimitw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgdlcsgj.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gvkoekwzj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gjdmaqjjq.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gbkmancmo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gtwuutdjo.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/ggkyreyzw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gwuhcnnmq.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gijoxsesc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.zdbjq.cn/Article/details/gqnrbyoeh.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gutynygxd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gxvyhyfbk.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gltwhxixr.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gqhmpaefx.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gxpbdprsc.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gkozzjopi.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ghmttihto.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqafhihxu.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gaczlcfmg.sHtML


<!-- 参考信息 -->