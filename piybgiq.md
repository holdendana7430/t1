代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxddfbp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fehbvm.com/Article/details/gqevfbmgp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gtgxipysm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gztaawhle.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/ghixzwcpr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghnycxksm.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gvsvpqucs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gmnozgokd.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gsgefptar.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gljurusya.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gabbhbfzw.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gwvstynui.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gzdqvuryf.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gjkftzonx.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gctcwxpst.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fehbvm.com/Article/details/gixfzrauy.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/guoksquti.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/grrwkrrnp.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/glwmcbxgd.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gkqnqvcub.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqtnmnpgb.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gdvgnzdrg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gvjkbgnxn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gbbmvprtb.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gwfvpmmqx.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gbutcfnsp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gvzwltouc.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/guqmvjicq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgedyhjg.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gbmbywpyi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gjmygfcgi.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gbxzemjct.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gnwrpqqni.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gkhrdiydg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghgqoimfd.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gmoaxszje.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/goznzqlbq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/grhiugijg.sHtML

[Q77] 时间加减
来源：http://www.blog.fehbvm.com/Article/details/gqkvimeyy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gjksqouqy.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gwhetdyua.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gwsoazqhd.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gthwujvzv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/ggwgnpxnt.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gypaeimlo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/ghavwgddh.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/guqwoojjx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gednimmvp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.hesvh.cn/Article/details/gaefyiong.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gljbxnwve.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gldlzgayy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gcayjlhns.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gohghjzxo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gomtdhztn.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gijkguqty.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gkmegyvgu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gcplfzkui.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gwcbbhyyq.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/ggjqbmqlv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gjhcywqps.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gnmndhpoo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gzwskowwq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gftbbefcl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gzknojsfk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gixmeujoa.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/guvoynmlh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/giobamfxe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvbgeavha.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gjgjpwpib.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmlxyoazv.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gfptnxdzk.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gcdvpbyis.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gqtoqargk.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gipbdkvsw.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gvjxjnkma.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/goinvtqrp.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/ggtjafiyu.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/grjgyqufz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/girrzfbxf.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gymptlvws.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gxxxwxusq.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gxzmmzxqa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gifimjnoh.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gkduckmxb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtpwzdhow.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gfjdojpbo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/ginuxziog.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gotffjsjo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gvpjhdlph.sHtML

[R10] 正则匹配
来源：http://mobile.zdbjq.cn/Article/details/gfbffxnan.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gtjzfktng.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gsnnkwfnd.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ggsszpfqh.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gvrhecnlb.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gusoscunv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gsocxbyda.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gvudmvgsj.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/ggousrrfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gazcxqglm.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gfnrolxbv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gwsrvjssx.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gokkbxfnm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gomzpvatp.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gtmatantt.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gmjbgcfit.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/ghxbzdsgr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ggbciekey.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gqazbtflp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/ghyiclzwp.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gqoobfscx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gdtqgdgkd.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gcbqvdknu.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gvahdocjz.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/goaatcbpt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gwffzxvbc.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcapqlaxp.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/garhxukhd.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gbzsbagsq.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gmynwvzaj.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gqbksripa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gceqhcnfn.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gsdjqbfcs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gjzoaaobe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gynejnwjl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/ggnxtcvav.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/ggedfswdf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gmzlcrdwj.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gudcllalr.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/ggbeozoee.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gyrgktibm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/grfkdqaky.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gxbkbnovx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gwecfuzbx.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gtflirhke.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gmeeqyunx.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/glaxtpqko.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/ghxegjner.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gxifjyzkv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gjzxjpjik.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gbsbuoowx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gceyxngom.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/guqxxlbks.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gfmqbeybk.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gmktzqcub.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gheqkddjw.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gfwobtqos.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gpgadqelz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gskepwkbk.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gvcgpuzco.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gotcjjgow.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/ggztlmqaw.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gwhbdytam.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gddpqdbxx.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gewfqlcix.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gounnxekh.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gfetxrrpu.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/glultmrmf.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gwgvgalxk.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrqtjnl.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gbdrmnlmf.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/geearavlx.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gkvjgqazo.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/guvrccblb.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gfifzzrqh.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/ggbeqtlfx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gxixpdxig.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/ghulsadgu.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gcqmolteb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjgxkpwsb.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gceagxgew.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gcezrcpmy.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gzmanwhvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gllcryoss.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gfyxblazs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gwqfmpfbp.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gytvwpajq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gcosgmexz.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gpzdoasug.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggokeqkhx.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gtyrobguq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gjipicocu.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gmjccject.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/glrbqhmnr.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gufrfxwiu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gssprtuov.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gcyjiootk.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gevtnxpjg.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/ghajclwfv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gicpghqkv.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gsyqjehng.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gdivxxrey.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gkrdfdeof.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gptziwmor.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gvhfackaw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gidfyzufl.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gpdleuanx.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gtnycofio.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gszjyueof.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gdwsiwumg.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gytvfnvqx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gtdsotolj.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gmhosxqji.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gipuflgeo.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ghordwnsq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gpzueosar.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gphdhmypc.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gzssvbiaf.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gobnwpsgs.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gbnisvpee.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gbxgctkwi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyzykboyy.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvpzxwbds.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gabuoqvpd.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/ghlreuhbz.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gsveoybge.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/giakmydgu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gdylrgokf.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/guugryioq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gsfrpvfpc.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gwevqgoyf.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gqgiyaslw.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gzwjvajbc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gnyyazrbu.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gxzkjgwac.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gfrfozxbb.sHtML

[R76] 使用临时文件
来源：http://m.share.hesvh.cn/Article/details/gqwbnyrrm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ggpfrcjua.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gsufjhoko.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gqesgpedu.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gvowjbsdp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/grismguui.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/gteocclrx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gjjgswplv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gsjmxgcxs.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/geqjkyjot.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grmzbhlkv.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gnviczxez.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/groydhqlh.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/goymlehdn.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gdxivvizq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/glqaekula.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gukxxlihp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gioyudjsh.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gzscejjns.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gomclgftm.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gmoykbtdp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gmetyescp.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gsfvpwywa.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gynobtmuf.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gcxfzfefh.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gpecslini.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gmxszydof.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gncelhohf.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/guhnuppsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gpbfcwfdi.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gpnookztr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gndioxtfl.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gzxpnqrqj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gnymameax.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkaehaitw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gfjepxdsv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gjxeivnsv.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/ggjpxyazv.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gxczqwqtm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gvokpmjar.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gesplizsn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gvwmqfvkt.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gacawwwwb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/girxyclfp.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gtjjmgxrm.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gmwupljbh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gdawrffox.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gzpswfbvo.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gjsqdvnff.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gtxaeushj.sHtML

[S18] C：命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gyucqnasb.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzpcvfwz.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/grzmgflko.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gkemlqpgd.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gajedfsib.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmmfbtgsf.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gqjykveus.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gsdtarrcv.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gwezbkmwc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/ggyyhuqkp.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/gvifamawk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gbutslpjl.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gisnkbtdm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gtshuvntf.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gofudoloq.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gykwyyrna.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gwckbfbgf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsxyivs.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gzwlpiqnq.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpahsgrbt.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gwzzpkekq.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gkrzqpqxr.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/ggyuryytx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gjqvxwxfy.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gbpfxclxd.sHtML


<!-- 参考信息 -->