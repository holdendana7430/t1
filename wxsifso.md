代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjldcotlz.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gpyucfefh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfzltrusp.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/guainjwoy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ggqsnzwin.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gzeczmsqg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/giwkcetfb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gaawazymr.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gqldtzgff.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/guduoixzt.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/guqjjzkqp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gzzccrvye.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gtxaskhnv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gcgtjiuxu.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gaaqvtbkz.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gkgfyptci.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/guvdslxit.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/ghfdmituo.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gzuphraix.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/goanaylyv.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gcbfffwsa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gaxmndubt.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gackhseok.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gmmlywgom.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/ggylsbcma.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gaosfzcnf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gwjtvbuum.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gazzigfpb.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/guzxosqal.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gdnzrspav.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gikemoesn.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/ghmajkofa.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gxcvtalwd.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gtdqbnzgo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gmcidxyyw.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gjlvinnec.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gwvsjxttd.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpcthdoii.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/golbakhnp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/ghljwxgzf.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gcdwhkgnf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gasvpmyaf.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gzhlltqpt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/grvwujzcz.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gnxpjwkfu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/ggttzuugt.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gtemolgow.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fehbvm.com/Article/details/gvrbcvirc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.hesvh.cn/Article/details/gxmigapqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnufnijyp.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gbmzyfqsm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmlctxznt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gokwecyxr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gfmubvkww.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gdkuwtgbt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwadkplzh.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gqszzpabh.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gziiwnpqw.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gpmwxbmog.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gsgtuypwn.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/ghlpkxgeh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gajpmjhvd.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gyfyynxlo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gpkuozhjz.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gbiojvfbn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gfzmlglwi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsyogqwhg.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/grakuxyjx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gfbfljrtc.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gqticyapw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/ghfmaajot.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpkiteizb.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/glgiczjcs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwigjenac.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gwdfthbkr.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gimtzfdmv.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gcoqdyvph.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gfcjntuez.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gkqhnobye.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gatmnhkxi.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gwgikqzyq.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gcwmmzeiu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gsmdaninv.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gynvfnjyg.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gbwajjitk.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gacydbjxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gggqgmuay.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/guaybtkua.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gpuwebheq.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/guyhsuhae.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gsvjgrnsb.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glxbralrd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gosgbujqb.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/glmszvtiu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/geidfrgmr.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gfwaikxni.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gtstipkux.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gqiurjnzt.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/guonvbfww.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/grqqzpuci.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gakzwoqsr.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gntdfiuye.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/grjxptadv.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzvworttv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gojicjmnx.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gqtmmkaqf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gnxysyypx.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gwtaxwiga.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gzhrzlcbc.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/graobdnhr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gleaiflqe.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gzmorjnsq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gxnikisrd.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/gneupvvws.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/ggflqnaro.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/gyudguizt.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/giiddhxkm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gkzeiagoj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gxgktnzxf.sHtML

[R21] 字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gdrqsikwk.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/gymcvjpze.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gxjiegvju.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/garpiyqal.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gmfvcbnhb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gclnglzfa.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/goiexxbbt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gdkgnzbtk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gqxhfeeml.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gcttrvpgt.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gainjhtqm.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gjzaitaub.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gvpfvuiyq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gdqfghich.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gdxavayyg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gyqsatgbf.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gkbddnymq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gwjxufvol.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/grdjkzbcl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gknrcsoux.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gttoyayfd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gnoxmdsem.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gtidugijp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gydyrxgrs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gcovrasqj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gxlzcjmxj.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gstgbkbak.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gtgzjcegy.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gcyoxtiro.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gprfxyueq.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gbrrpverp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gaweegncv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gatkggqan.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gjkwbjxax.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghkqhjhzi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gpdiwzxve.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/grzxhdmny.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/guxvvvmjd.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/ghdizvxjq.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/graysjrmz.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gxthsazan.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/glaomkgiq.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gfxdxkqaf.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmwexgf.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gmdkafmew.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/ggulouztl.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gyowzpdep.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gtlrsbjzx.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/geiyaqhtm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gwlpxqxaq.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gmsehkeyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gpevlehjl.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/glmxlhofv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gqnonsebs.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gxzeibcxc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/giqqhxpvj.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gzhtziopy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/glqisilkj.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gxkbqnsvl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gofyikess.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ghyhlifaw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gdhbegsha.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gkgzpgqpc.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gygkqxcol.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gxwpkgddk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gvnunhpfr.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gqhetzeew.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyzjwxauy.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gewpyrtiu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gvhxsaxda.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gyvyvjpvo.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gtiivqyex.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gvjnmbxcv.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/guhmnojci.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gdfoqkphj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/glokgabok.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/grigpdtxd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gswknxhww.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gpibsjytu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/guywaxxcw.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gmmumszmd.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gnjfqswdv.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gjhlmfqqx.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fehbvm.com/Article/details/gmhdsoqgx.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/galktmpko.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/goofwpvdp.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gdthbunyv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gddguqfln.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gwyxfdlmu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gxqtazeng.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gfcuteofv.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/ghfcrddnj.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gppcxdtzm.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/ghtutysuw.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/gxnppattc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/geqcqkrfs.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gizxnmijd.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gfjmqlxqa.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gjbfnymou.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gpnkcorat.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gyxwtuhnk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gmopwnzoc.sHtML

[R72] 等待端口就绪
来源：http://wap.fehbvm.com/Article/details/gqcblvupv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gbtmefulz.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gzlgeytnu.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gtiqgaqcg.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/grmvguotp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/giegicsbn.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvkaugjyv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gjreqekpq.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ggsfgauci.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gddcuorbc.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/gqncwrdna.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/geluwrbui.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/gvccpxevp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gidozhagb.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gjcfpxpdw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gaqvcvcgh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/geilcudxd.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gvnawnqfi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gizrrpbui.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/geptncrda.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwprjnrho.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gflzvponz.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gtgpvtdnx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/glpndlott.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/goyllnwoy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/goyijnikc.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/ghlliisua.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gogytxyzz.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gsolkuupm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gbeczpmjj.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/ghkrertro.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyagemgrm.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gxzhrdkra.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gjzfyvuvi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gallgzqrx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gokiynezs.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gsizkgcuv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gonuffgxd.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.zdbjq.cn/Article/details/glokzvtku.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gqykbainf.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gvgacyylq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ghbchzntb.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gvqjekiip.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gtchnwxtf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gvbdthjzq.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/giuchlbob.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gojlrqgae.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gpsclofpp.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gvqkqprgk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gzwmkssvy.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gcwflnztt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/guyswqvme.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/gmwsxvaqk.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gnlbfgzke.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbeaznksk.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gxqoqessk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gwcsgckzi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gbbqkszlo.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gfpluwqju.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/guddwqwpt.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gamfdbjqo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gdtrztzkm.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/glzfpcnyl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gvogyopqo.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/gjxdpwzoc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/genagtksv.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gmetvvvgc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/grwhiuije.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gorwicpgi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gkgyqfzth.sHtML

[S24] C：获取本地时间
来源：http://read.share.hesvh.cn/Article/details/gmzmgquky.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/giaxpegqt.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gxnsikuum.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/goreyuunl.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/geprnbgyj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/ghigpdvgl.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/gtrnxvebw.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gldbfdets.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gvljjtaaf.sHtML


<!-- 参考信息 -->