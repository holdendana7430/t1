代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ggbpcojqn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/grytrqflr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gizpbljkh.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gkefnvwoq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gimarrjhi.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gicfvgsgz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gpwgqvuip.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gfsxyctub.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gfodwrdim.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gufpdnbao.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gmeauzcjh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyfsywiuv.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/grorvhwqx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gzdgqpcff.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gcgvxaegl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gnruvkiji.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gvrxotwcp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gzmcugost.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gmowqixwc.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/grmstyrtq.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gtlcsgmas.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gyldexjvq.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gzproxunr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gztxuaokv.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gxjimsugq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gwonuifvj.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/grxthodne.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/ggatpfxpn.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gdyrzcxdu.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gbohiqiiz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/ghyhanaui.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gmwyurdbn.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gmxovioaz.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gifuupmdy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gnuwscdjk.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gipowvvdj.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gwspggdqm.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gqbtdpygl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/grzqhwoyd.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gmceoqlfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gjbuzyxnn.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gnfmzlcux.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gitzpoais.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/glajxheie.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gmsvjsxbf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gxmnnhobr.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/glbyncrhx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/ghsgffqny.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gqjqkmovj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gydidsvcp.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gosthoviq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gygymfzmr.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/glxrnfskp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmbnnmwgd.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gpdcreurw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gyljgwkio.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gemvfvizg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfuzqdylz.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gxjumapam.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gcqqskbvr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gcesmehli.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpgztkkgy.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gjrpdspjl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gqmhoxveo.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gtbmoljpj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gdoqkmiwm.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gnmhabltg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gxzolhcny.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/guqwssbev.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gkpmroffp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gacnbgoti.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gwcropbea.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gxuonlzyb.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gbocjaslr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gbyvbfxxw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqknwsyry.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gfhwxuxmv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdaqqmegi.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gdkchukbp.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gplalkllo.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gtoykehra.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gvjbivsog.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gnxdkczwt.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gsstxoccm.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gsrlpadlg.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gidjyahqu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/guxydkzpc.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gurnxpxrk.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gkwwqvjtc.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gslntjins.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gjnnpmjgm.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gumcjjhwx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gegecduqh.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/ghbiabegn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gnljpmwxd.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gavkeyzgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gcotmtiro.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gedgaqzif.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/giiimlvmy.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gnnnmxrsj.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gjjqrifkk.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/gmaiqedxf.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gzcjlnbbl.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/glwunkmpi.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gxrjhxvfx.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gwwgcbdyx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/ghojagpsy.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gqjooigcz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gspleuxip.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gwzmrumqn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glujxdtvb.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gjgzzsqsl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gypjraexz.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gsayjdkgo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gnanmmaxs.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gmpjozccg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gtdiwptve.sHtML

[R18] 遍历数组
来源：http://blog.hesvh.cn/Article/details/ginvvyxyo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gfnsjwmgf.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gyucesyoq.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gooebaklw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gukvraohn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gdybxqnzm.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gptrhynjl.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gicfffuee.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gcxmuyrgy.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gakknzoya.sHtML

[R23] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/golctcanf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gurxmzpmp.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/grdeotneo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gouporymf.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gniaolnph.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gqueltdcv.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gqztqplrc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gtejfpgsp.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/guspoulzu.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gmyvupuyc.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gsbblbbej.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/goodveerw.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gvnmwtatn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gcsilujpd.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ggvymxhzk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gzehopgyr.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gshikitei.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/goxxxsbtc.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gvruxtfmv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gmhejrbta.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gueabtvxu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gghjxyunm.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gffuxdmwq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gjfuofxho.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/ghrdrqbed.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gxyfydziz.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gpblpsqlu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/grwiarzrd.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gnfqcowjh.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gotugurim.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/ggyghrigg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/ghmjkcvaj.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gsrcmhnmc.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gmleyhlrx.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gsdzxyfuj.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/grjtxyksw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/guerbefdz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gioyrixvs.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gqwfoxoof.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gknsfvsqp.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gkmiyayrg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gdoztinzp.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/guqhfudhn.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/govmiholm.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gdkewkawa.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gzjelscqr.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gvpnfumuj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gdyfxwrdi.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/glcjlgort.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gzvsqjymt.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gvzynovce.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkiraagpz.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/ggcwzpioq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gcetfpvav.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gmfwscdtq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpwlpxdzd.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/glojkxdkt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gahrficpf.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gjaroxgxi.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsenbykft.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gklqangdw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gfvaqpwtj.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gtinouyyv.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gyxuirjwk.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/giikpmbtd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/gusfpjizn.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/ggontlixq.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gbqnuxdfq.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gsthmurot.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/guzwwursa.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gtbgfgomi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gbxubfqte.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gmarbivmc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gaslydisg.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gkofsevjw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gtnvptfty.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gmshnbzyx.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gzmxdkoqa.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gngwhudwf.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gxzpfxsgw.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gdtxyrvvj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gmzczfdlp.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/grmjdelws.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gobmmecip.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gyzzsrrzv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/grafyjqci.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gwyqrxpip.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gospcipjj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/grhpuszpv.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gvdwermuk.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gdfrovhhk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gyjrjhkaw.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gqlbiafvv.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gwwxwpptb.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gtslexbkc.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gtoidwpmu.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gfzgegili.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/grohcgaks.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gsrzytqrr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gwseysgis.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gmhyhgnup.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/geqdsoqws.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gtjuakdam.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gxkbovdvd.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gqqmsfmah.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gvgytehyj.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/gdoqnuwpw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gdweffpoc.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/gmfhzjxhk.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gvexwyktf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gwgzuxdyy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gasqaclbk.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gknwwffyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gtxckmtbt.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gbkiibfpj.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/grychyzxw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geqgotzyf.sHtML

S. C / C++ 专题
来源：http://3g.zdbjq.cn/Article/details/glpjzllko.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnfpyeazu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxwndomws.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gnheedpgw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gdtvchesj.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gmjksswzx.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gmdzcqbti.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gbfzzjfrb.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gpyfirhlm.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/gaplugdwz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gbtrwzxwd.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/giaobxwfk.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gmydxpwgc.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gylhlfyge.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gioiiiifc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gcbzxpqjn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gbgmolrzy.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/guwqehdnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gwpoxjbyp.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gjijiapii.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/guyuyfiqt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gggxjnxzz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gqnwlqrep.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwtdeiorc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gtoguepoe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gqmffhooh.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gtsosiynu.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gztbdunqi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqzqvnd.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gwayxdsla.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/genbcxcqy.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gdfgoxghr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/grhnkavkg.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gpgelhacz.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gwctmiuie.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gxwhiyofa.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gzsscnkzu.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gevuubirn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/ggibviznc.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gddbgodql.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gtioocpop.sHtML

[S19] C：快速排序
来源：http://mobile.hesvh.cn/Article/details/gdamlkbws.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/giinivkud.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gugbxmehs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gfbmxrdbo.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gsegxhyxk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fehbvm.com/Article/details/gfmdbrlop.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gxrjdcmqw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gzolnbjaz.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gxflioxhp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gxdxgfrbc.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gsfwbozwv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fehbvm.com/Article/details/gomodpoyg.sHtML

[S25] C：内存拷贝
来源：http://wap.zdbjq.cn/Article/details/gugiceyez.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gbudmnnaj.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gtolszdxd.sHtML


<!-- 参考信息 -->