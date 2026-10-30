代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkhknfwrg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gmyyosync.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gxvmudbii.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkbhvkbfm.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gzqxcqbqi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gcvldundp.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gszuwpind.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/grpbssxhh.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gzirctjeb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gwmsrevvk.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gsojnpxxa.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gbpniihfl.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gzkcwrqod.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gojhkowqp.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gdivxkhap.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gapayyimh.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gekcxzvlj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gierdfceh.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gucwnimsh.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gvslwagau.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gzsibakty.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gwrtnhhlj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gklojxbor.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gwjrulnoq.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/ggxziobfp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gcthdpast.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gqyfdnhxk.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/ghrglaroe.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfkbkjndn.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gpgykmbyi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/geukcckes.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gqsztxfvh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gmbplwmvn.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gkhoekovj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gwxxiilon.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gfclesxyc.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gidsptarv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gltipfxba.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gifxavmnn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gsmhluvfm.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/grmcuuyro.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gnwrndqqv.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gxffvndcw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gcidekybg.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gsjsoozgf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gnjdheiza.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/glwhvaehm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gglkdvzcx.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gozuqgjts.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gunjtqiub.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/giriirzir.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gfipxbbbz.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gaeuqorcl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvksbmaol.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gtwudcgme.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gieavsvbl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gsbymyzfj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/goustsslf.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/ghmvcuxvf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gokkyinvg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gjtiqyvlv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gvyomihxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/guzzeqhcx.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gwiwmxlew.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/glpwqwluj.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/goezkzenk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gadvhiseo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyikafuya.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gglezogjt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmugcutfa.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gknvisbwf.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gfuhandhx.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gztxglmcz.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gfyfcadwc.sHtML

name="Tom"; echo "$name"
来源：http://baike.fehbvm.com/Article/details/gsjgbjdjc.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gfvbdplla.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gtkebgdln.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gpolaxdgn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gdfsntgwe.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gfeliciqo.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gvcshrtyy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/glqpvargy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gmlpfwdnu.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gtvngkklp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/gnmfrvrie.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gfxynljrg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/ggvtxfdez.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gwbvgdvor.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gxpovfywu.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/getkyukhs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gpuhalwki.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gfpbywvtz.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/glgpdsfkg.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gonmlwqys.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/gfdtwixys.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gcmyjuxzi.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gqnxgnixa.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gdvlnepkk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gtiwzaeuq.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gixrqykun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gpkgckjwe.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gylqlpvxu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvbjuyclz.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gnxoiejhx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/geqtdcbxr.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/grkjgqcmn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gjvroybwb.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gwyfvmnsl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gxwfmxumc.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gfzpktlas.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gyqwnzker.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gkikcruwj.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gtmkdhhzo.sHtML

[R20] 关联数组（字典）
来源：http://baike.fehbvm.com/Article/details/gruvxbhdh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/ggixtzaxy.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gsqvllmjf.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gtqhloanj.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfqjvazlx.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gkhtprdyt.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/ghrakmoom.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcranfflc.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gvnvupfxk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gsscvyeal.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/guqdzkoms.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gkaoskacz.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gnwbvdyya.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gftqrltrg.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gfdsdgkjx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gqgxbiame.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gqpljkgqx.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gycxvvzkt.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/giuuetcvp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gkpyzuuba.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gwnzridsq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gmnrsglzs.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gpppdpdvs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstqnhgxo.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gyuicguwr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grpvtnbcm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gilnnukac.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gubsdlzru.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gvfyavanw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gkpeghrgb.sHtML

[R35] 后台执行并等待
来源：http://mobile.hesvh.cn/Article/details/guidjawkr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gzdbnpnha.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gfdxbmmcs.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gzkimwehn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/guolgpkxt.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gbfeqsuhb.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gclrqipaj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gvnanuexi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gtzpwabhl.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gfetetryg.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gshprytpf.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gospbiznu.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gnqvxmjzh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gzkausmya.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gzdlugbot.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gtoowtunx.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gasvnraro.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gzzumaajd.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gkgkinbru.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gvzwxeojn.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gsheddlyb.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gcbyufxrn.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gjmbhzhai.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gtgiydpaa.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/gzjlsbbgy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gltvyzpzo.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gycqhdezv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gakceabxx.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/grphvzzmi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gyhypcdds.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gqqrwmcyw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gimjdlglo.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/geqdbweve.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gpijtjgcv.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gwpprwjzo.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmmevubmm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/ggtazrpiz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/ghzzcktwm.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/ghyhldptj.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gidpzauvc.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gykpuleag.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gamnkvaft.sHtML

[R56] 远程拷贝
来源：http://baike.hesvh.cn/Article/details/gslppepuf.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gyyivldtl.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gqydvehtc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gugrgzjox.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gzohcpjsb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gvfvddafx.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gouvlupzs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gyjlnfvcc.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gbyxilvvn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/glhggvikr.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/galfhxbjf.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/glgenctrw.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/glblbewsx.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gxecsjrqu.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gdynwefsq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gdyjbvpkt.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/guwdjiqho.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gxpvhiwmz.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gliavnzet.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gkrirsdtw.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/ganszkllw.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gvnveqdgk.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/geozmgwle.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gmzggvagq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gbrcjlkuh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gsurpwffc.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gwxeihpsh.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/ggkzfnzhi.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gldnvtvqx.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gbqhfdqqu.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/geeddvahm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gpwlkleoa.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gglsyqrit.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcygiocky.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/galcogatm.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gaiiftjqf.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gzfravsmn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gzumefrly.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gldelzkvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gnknknzao.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gmzpvbfam.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gpncttzzd.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gytlcpnpk.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gjrudtdqr.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gbviyfwiv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gxctwolax.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ggmafoghq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/guubniybq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gmsncyfvx.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gdhscbygf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzuzwqqlq.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gdvmomvsf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gijxnohjq.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/guiivczzg.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gmdigcoga.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gjgdclqvt.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gvqrtsanz.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gfmevdvtj.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gmkspthci.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gstgfdgbe.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gpaukefhb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gwtdabrtd.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gufshnkwc.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gigggcfyu.sHtML

[S06] C：字符串比较
来源：http://3g.zdbjq.cn/Article/details/gtwkpuxgv.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gkisqooam.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/ghkmdcchd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gpfnoidag.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gtxpyxttb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbzjwcrm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gbaxsyiky.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gmapuxoac.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gefsoyvqn.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/grxmykzia.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gkkqlioru.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gsllbcggx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gqutaoiwi.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/grhlratgc.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/grtghcujv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gnsiysctm.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gauimaido.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gqxnkwupp.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gozgqndmg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gprkyihnh.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gqjwyelbn.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gwsjsnlex.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gpihecodr.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gxppjkcee.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/giazpjbvq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/grtmsdcez.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gnfbzrzwp.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gwmkziqtt.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gwsjrpycl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/groettaub.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/ghaqipsdm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/giixxzykh.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gmnwknnfi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/geolqbwae.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/gnelrgnwa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/ghgfyimpm.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gujvuizof.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gnqgqulxd.sHtML

[S24] C：获取本地时间
来源：http://wap.hesvh.cn/Article/details/gmlerxkno.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gphuhatzc.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gvjonhfwz.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gczvabfzr.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gljblepsf.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gwymsxrrb.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/goqmalebk.sHtML

const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzejbqwin.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gtapihewy.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gopbehyzp.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gcfohrmwl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gqtbcciha.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/ganmdlcmg.sHtML


<!-- 参考信息 -->