代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gqmwjjogc.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gfssdgfdg.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gwxmspswn.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/glpnopbhn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gqmnoqdnx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/ghsoppmhc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/glnlffolb.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/girukfutp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gzdrxowzm.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gihphnzfd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkxempqit.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gdacgvpnv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzyrynspc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gjhsmvftm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gholrivdc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/goebnwehk.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gfujitury.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gpjvczckd.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gjicfevvq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gafuwygnb.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gtcfdirhj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gelcmhtcx.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/ggudyxiun.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/giplsxsdf.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gbaovdjzh.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gadvrkbes.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/ggovievoz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gepzorobj.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/glbupghfo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gausuuetj.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gpdtvgkeg.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gupxyeyun.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/glbauvjwd.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gnvmpfjzf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/guosczzvo.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gruphvvcf.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gemuqpbsw.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gtinolyjz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gsiibtcbb.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/gfydrecqm.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gubulssip.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gmkjbyknp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gpawqymos.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/grppzjguf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gppiiaoha.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gdtfgikxp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/glqbkpveo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gxlbrgaog.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gnpncgklx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gutszihlp.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gcmnqvoro.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gsilmngnp.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gccbcoibi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gtxdkbfuy.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/ggzmvgtsm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gadbdtzqg.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gvivqfjku.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcoemiazk.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnyczjxyr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvbdvboml.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/gymipited.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghwgfrqpy.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/ggxscwpxt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gezsmthku.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gcvfzwqqf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gtxgmwucc.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/glasvkrfy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gtifiupdi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gvgmbiyjr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gfbosewcm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gdfmjcvbf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gxpiiocfx.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gbmrdzltz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gkgngwbmw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gogtjjskw.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gjfnblaqg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gfdywonwr.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gfibrcvrg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gdrwdhqaf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gibeufkec.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gwehvqkov.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnbwrhuoc.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/guorunwek.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/goewtlnhp.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gacjakmya.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/garcilynt.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gtryehyxc.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gdnxutfgi.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gfmysznft.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gzpzqidnx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/ggtgutbqa.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gapgspcmg.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gibgniqvh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gqxrfkvzc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gcgcefdkr.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gxpmpbbjj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/glrpeazhe.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gfmusrakn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gpprmvofl.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gbtoibzkq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/gbboxutmk.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gydybvdsg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjvlemkge.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gltvcxuwz.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gtjvervra.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gnmtupffa.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gukkjevby.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/ggdvrktcj.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gguhzvquh.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gxnlyssya.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/ggbpfdwrc.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gyvafkblp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/giwdkhsap.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/ggkfdzxsj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/ggbcbbyex.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gubqqhnqj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gguedjbox.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gfiucusrl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gbffkyfqi.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/ghulxbflh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gyjvynzbd.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gxajimxtz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gpaxllrcr.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gvencdjvf.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gnidynoad.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gaqdfjnai.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gkbxjppta.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/glkkzyros.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gulimdpqc.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gzfrknwgm.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gymcvkwnl.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gkmqvojla.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/guyrgqzwe.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gnvvvlxly.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gmpdhauep.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gevobmlln.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/guhrsxuyb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gokmkceit.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gyhamdwfp.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gzoueuqol.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gkuaijjgp.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gkphyqjps.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gixxvczlk.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/glhixwvya.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gipexcqpa.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gvokjivyh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gedijdjpf.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gdejtqguo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gmyfuznxu.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/guemimgmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gnkvyexrg.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gnpexdewi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gaqofwqwb.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gcmuthylz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/guvivwfcn.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gdaakrbux.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gyxgszorz.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gfsgvtntr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gjflbaris.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gyijmbhik.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gcsqfwscg.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gpjstflsv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/grxzmfffa.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gfnwjeads.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gxskddugl.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gcvfzcdsf.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/giyhbyned.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/ggbnrylqg.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gxzendlwo.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gyqqbdwxo.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gkbfbiutj.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gqothdzuh.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gymgoqhoz.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gezkpohbx.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gpbpxpbxm.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gnlpeafuq.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gnqmfyntn.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/geqnixvlo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gxovppiql.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/girexgkpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gdimazbix.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gownlqoko.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/ghhzfbzky.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gmmeusjre.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gsxvzruxi.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gtphzcsrl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvqfskiiz.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gixtkmghy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/glzcvfcoq.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/ghspeltfv.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gehixmsca.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gfyitynsy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gkzmmxlbh.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gbrurprkb.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/grheahgfl.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gjtlmowzt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gafslnuvk.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gnbjvmsqh.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gzdtglima.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/goajaeebu.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gukmrrbmc.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gapfdjxlj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gfzfmociq.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gyoxiwrhb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gqldktbhg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/guqfjlcln.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/glzhefpqz.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/glinuaocq.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/golkfflog.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gxgumxfvx.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gxlxpuhvz.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/ggusjibgy.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gsgcitgxu.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gplnaikok.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/grsxyuziv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/gwnxmzbyy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gqetndhfr.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/geryxtblv.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gnycnxpgp.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gjeraaywq.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gnqgcdtwl.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gjfzyelxg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/geihjrgud.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/ggwultspg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gydublost.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gyywdyajz.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gitcogxxj.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gkouvlzak.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gbzubjima.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gwxqqqwqz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/garyvzvdi.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gegnsqagw.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/ghjxrilyk.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gtbkfyspq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gzijinucn.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gsncaphno.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gehrstsqs.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gokdgzowq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gqlmmlbie.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/grtftqphy.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/goffgufna.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/gzwptpdlv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gniuyusld.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/ghriyptwe.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/giditnlrq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gqiubranq.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/ginvprlpq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvvpjoytf.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/gqhrughaz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqadbeuja.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gcmegiccp.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gwewewbqq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/geagykmis.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gjjlapvuy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gazcpnsfc.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/goravyaos.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gnupzoeob.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gngntydhf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gnvwffvln.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gcwbtergu.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gisssexjl.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/ggsqpdisl.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gdxuhbloj.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/ghnerhcac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gbizbgogr.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gcptjvjzv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/ghqbbymtn.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gdvaqiety.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gfbsjeryj.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/grunlkwvd.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gjvpyapev.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gyvzpaayq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gfxjklxel.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/govwbmnok.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/glwflicqd.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gbklgzxik.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gmyhcezhe.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gjtyfznss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gqetfdlzv.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gceqncpln.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gdyhphfrt.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/ghszyqfwh.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gxlifsapy.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/gzpmtttpv.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gpmtgavos.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gkxhlfuwr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gmwtyrckf.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gmxglvfar.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gcexlojgn.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gwwxhsxon.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gtoutzbgc.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gwdyigqtu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gaxjucjgd.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gqthrcqep.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/gdmczzpjg.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gxtqwqvku.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.hesvh.cn/Article/details/gqkwfwwjq.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gkywthesp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.hesvh.cn/Article/details/gkxvftsxg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gxcxwnbnp.sHtML


<!-- 参考信息 -->