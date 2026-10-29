代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/ggklpopct.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gjiwewnix.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gmhlepsdw.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gfjwjtmxf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gppjmemhf.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gtdwngcui.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gexctzslw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gaoxwqgfd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwflvrwif.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gcrpabevm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gtxyebrym.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/guotmlmcc.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gfuncrlkk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gneblouoz.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/grtaigpqe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ghnaydlwx.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/ghaebcpuz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gjzoxoeoy.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gmleivahx.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gjkdnmzwo.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gyqbdjgud.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gtgrsnexi.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gpjkvuzhk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gxrtmhnno.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/glnjzfgdg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.hesvh.cn/Article/details/ghbnxxtzg.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gfwbqvzsr.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gnprhuiqe.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gyxwgzliu.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gyqcflocm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gavfimpel.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gsupexefy.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/gcxnoproj.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/ggqdimfko.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gjnjrtulc.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gbpvfwcyu.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gaxrrxsgu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gvoxmjnhw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gxrfhajvk.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gbtmjowbz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gwbjzlyqj.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gduzziekq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdpnnzmhk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/geevzvtjj.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gvwoqctkj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gdugojyrd.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gnkzyfysr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gftklinlt.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/ghfsoituo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/grnuoxvvh.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gwwhmousm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gukllyfvj.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gqpafwnzu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxiwipccg.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/groeohbll.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfjhzyjqa.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gppgabxuf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqczjzueg.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gyziiriip.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gsnowqjcy.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gpngswked.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gchvehrsh.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gnohfpuut.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gebjpbidc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gqwvkwxyg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gvwafdhlc.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/ghxdcvuay.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gcidjyswe.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gfeddfajn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gbcqvhjft.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnriaafdr.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gsocgbvgd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gcmwouzmb.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gfuyyslow.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gusuthesi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdjnjctxf.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gqetybhde.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcnklbgou.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gdwayoysp.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gxqrnunah.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gzrdlenyh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/gkibwbxab.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gkvdnlmdk.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gaowcxyvr.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gwiykrwtv.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/ggslnmvny.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gwrfmegqq.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gdckxntky.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gectqcjyk.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gigdjqqyt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/godoyaifz.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ggobxktmq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gktbgebui.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/golnyieew.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gwnounuwt.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gdntyzauf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/gzbjpfsgk.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/ggksxpiep.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjknbeehi.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gelawxzrz.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gkdqqpyel.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gniauheea.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gklawvrho.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/geeyzrxtz.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/giowgovbf.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gjpdxvclk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gmuarljcy.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gcrcfpfjj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gmvrcnpxh.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gtewuntmz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gkphoxlfa.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gaqvoknjs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gomridebk.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gkqbgxlep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gwxxomgzo.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gorifhdfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gslexyrhk.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gnlktwuls.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gvosddajq.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/ghzxmovbo.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/glbshpmck.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/ggwmelzve.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gfpjshzuo.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/glqcepdmp.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gpxlnwhoy.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gafydwnio.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gilpalewt.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gahsdrsof.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/goelrplge.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gsgnttnzz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gbxqvabpi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gbxqyeddz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gubwssrzi.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gxxlzeazp.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gdzcxhdmp.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gabgzoboi.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/grgzqnpuz.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gtolxywjg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gissqljfc.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gwpszhlhw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gfwybhkmd.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gcrrtyfvh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gwiztgusl.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/guhlhebzk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtaazhzjn.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/ghplkjqod.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gedqdfwic.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/ghcsxuodd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gqfsufbqe.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/ganfdgcod.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gayifvxfe.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gjkpnbvfr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gdbcuzcta.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/grexrnikx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gwxeuhnfv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/giqpxexez.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gxbczamjw.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gesqnyxrx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gsltbxdkj.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gjejikdei.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gefwvjxlp.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gjvksgokj.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/giwplfvba.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gbvpngiou.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/ghrxtrlip.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gknjlzmru.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/geeobtusm.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/grdwirrto.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gzlhjvnjr.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/ghwqcmskn.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gmlkwzrtf.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gmvvjmarx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gfkkajruj.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/grsegpcdf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/guemnnoyg.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gustxazeb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gbhrewedr.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/geldsrpln.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjptewlve.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gfdqvllvz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gizdyzkdy.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gyzwoudaf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gqgwdgkcn.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/guraaqljm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gtatjrgih.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gsoogqroc.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxnowur.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/grfxzwpzm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gatlxgfad.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gsuphjmis.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/ggvufgdqh.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gxfpvvjwm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gvwmcsywu.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gqplgqsll.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gaqmbgqqy.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/ghrcojiqm.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gdcfqbmda.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gggrgxvbg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/givccqmck.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gvjlekfiq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gzmqfmjyg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/grqsvgjpg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gwdzichoj.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gskaaloon.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gbisdrmov.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gmpmonjad.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gskqecjfc.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gzugcvsqn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gwgrqjfev.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gvaugtiyd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gxsjxnedr.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gxjuxgggf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gjtduqqrq.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/goietbums.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gerpiqtql.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gyarakjjk.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gadftwmvz.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gkakgfjcy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gqtkxvuof.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gfjktkvgh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gwqoeohaa.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/geawksljr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/grrtjplwb.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gizxwxrri.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gghklcilq.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gmiagykju.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gdwuxrvos.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/ghvggmkxs.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gtoolalcz.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gyorjtfir.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmjtyfdpi.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gtuwyitip.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gvrdmvoes.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/goswtogah.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/grslhpyqw.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/ghslredqh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gkstnrwem.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/grncwzuls.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gfebrfuov.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gcsmobmxg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gsdqnncxn.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gvuffxbbt.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gwjowkrsb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxopygdpl.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/glxmuxqxl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmrkpmqnx.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ghhxkvqcx.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gicytilty.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/giupqwdip.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gsbezpfoh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gwswcscfk.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgldnsl.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/giijkbaxj.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gppbzzjcg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gpsxxknid.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gqnocvpla.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gkdfrexds.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/grkyrtuqq.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gutsomzxh.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gjvjffpgp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/goyqymwxz.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gqebrkmtv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/ggpzrdqgm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/ghxdcsejv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gofupxrpd.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gyzqzmbxh.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/grgpzvgmu.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gcotpnoge.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/ghjpcouxi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/gyckjqaus.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gyzttslga.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gjzaspnxb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gncvefipx.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gbdkcgbyx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gfmiwfbls.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gsolimwue.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gdmtbjvwy.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gekjtpvbb.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gogshiucf.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gczeplmor.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gptbgittn.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gwhwbvqtj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gwmrqquwd.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/guuckmeap.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/grfrfwvzf.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/grmdfloqb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/grpcrfphd.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gdggvgznp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gijuqctzf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gurbmrnon.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.hesvh.cn/Article/details/glimpsspa.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gtwazczvw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/gaqaetrqh.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gwnftaszx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ghqyndrpn.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gcwvqwtfj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gcievhges.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gsgqyiwei.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gwziroqzd.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/gdxpuaadx.sHtML


<!-- 参考信息 -->