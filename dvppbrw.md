代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gcqpyiwgt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/grsemzuna.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqedrjvkc.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gnxkkylfr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsqfzdmq.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/griuhyqpy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknjxtbgq.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqxcwlts.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxdmriye.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gncinefvd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmpjdhpb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzvxuotuz.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrnwufqd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnfdlixq.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhwlselw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gvcntrmsy.sHtML

[Q63] 开启事务
来源：http://baike.fanxiaobao.xyz/Article/details/ggutgeyrr.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gsjhuusgm.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhgusrbk.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/grwbotffw.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gloudtops.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gkgpymqec.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gunhpafnf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/goymlmiug.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/giwpfcvqq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvajxznk.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/goxijpnda.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkcoeauu.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggncxiqzn.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/goyekvwgb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayplkdrh.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gsikusokk.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjzfewlzi.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshdskviv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuumvfbj.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/glehbugqi.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlvvktta.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnkpftwu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gwvvidoxi.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxomitqc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/gssgwdnin.sHtML

[Q75] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmaekdor.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdijwgkxj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/guudanycd.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvwwyztw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqvedszi.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwzkgukw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gmclpsxvv.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/glohddkye.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gpmnwekxa.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitwaqnoc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/geudmfrgl.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gzipmblhs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpgtrbxte.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gltphjvyn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gaqseevzn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gtsatxbqj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glffmnmft.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggexppiiu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/geopqmejc.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/giuwjgezl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdltuzmiq.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gsajanzxs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyslpzwxb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gcisvecgt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gyuswckll.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gnbrododz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/giuvkgkne.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gawfbbufi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzhgbmkq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmllvfjks.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmbqwbgu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcyollew.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpisgunf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gulaiyswt.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ggjtfsudj.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gkgjgfcqr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtqepabc.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpynulgc.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gihtxhnsn.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gxykrbtoi.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyybujlly.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gqviydzho.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/grxndosuw.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gphaanvll.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/glqbqxfmg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswzssuln.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyzjbcwl.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gotzsthyy.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/grbkkacap.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghysraotj.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gufxilafn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqreypyf.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gskhmyvac.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gseqmpnvf.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gvlpiaqgt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/geqduzisy.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gnotrjzkv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glrbkpexp.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gwervllph.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/glxfszqym.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyokorja.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaymbkjr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gnqahccsp.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcldanhx.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrwizbjr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gakdkwsll.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcgtflug.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmzczkzjz.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gndshorxw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzhzkeuu.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gserhivft.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbartnmbt.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiegopkn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grbdgvzlk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzlogypd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvxmdlxj.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gdmplnfzc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gcwurknbi.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gifcvqiqe.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwwtpksx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/glbhgxgia.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/giezpprjx.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxthawhut.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gutvszibs.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gylvuzopg.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsnyqjqcb.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmwtvizf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmjeljhx.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvprbvauz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfxjzlje.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gsfdfztrj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbydvadj.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gpocvanxt.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbeqlaemr.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiiuegty.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gmipufcwe.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsdecjcm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gafsvsahn.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgftifdj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdrozzmd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grttdvrvw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gcuzelfax.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ghyqrnivl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemndssjy.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gincwnupz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guuchiwod.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvtutrei.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwgxtyhp.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gerohcpvl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gkmxrtwol.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/glichruuz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxckopefw.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaykzwbbj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkqfyygv.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpvrpifbu.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjyadbvkx.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbwrfhgv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqbxktzbk.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gwnayfxiu.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdehqnzxy.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvkkoxspp.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorhpuhdl.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaoiupec.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlxdvory.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ghkadegfd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteudffmx.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glsrtdbvp.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gexhmeiiv.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/giquoocxf.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/guvlbvpas.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjjngoch.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gsajspfqs.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gdsrrxynf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/grkykmtfc.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjhemtfe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghtwnagwq.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcsdnvdk.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gafcxoywe.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/glwmfjgtt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gykolwebt.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsinjjet.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflrrnyny.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gbsraxfqd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/geqevytmt.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gylnlxfbg.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gmozqutab.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/ghpjvuryy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gqotvrgge.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgwpnrrt.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gnwanjglj.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gydijxnrp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhfhkekk.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gwatccrmp.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqhsfaem.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwlgcwoh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcqngrrv.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtwyrbjp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/ghywmfpdb.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gmoibvyru.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbknkmyn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmswdnqsn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtssdiihb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjqpqasq.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gunpqhkxx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaqsqake.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvqisluu.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlsycjwt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbcxnfkd.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpmvczig.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/glcafkiwj.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gusilqrki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsyrtgyl.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gelkhkcky.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/grvafrpff.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gnyrsntwl.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gvslxpqvx.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmkqwioh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtbsiztt.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gnlzaqroe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyyjcdqe.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgayzjkc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/ggdnfumfs.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gvjempkfe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gkexaytkx.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrdybyog.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfwcdqcd.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutzblpjo.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqruqkuq.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ggyfmszqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/godimkqax.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnsjxitc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzhyammt.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjdgfytrm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gpkuxgkqf.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gyitmthed.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gftenoimh.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gywfnpyxn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfwfmnloe.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gynkaplcl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzgzapfer.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzpbhgcu.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/guqoxevdv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gehiawiok.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvodntod.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxpfgueoq.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyjtxhmps.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gtotsbpys.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxjyltcc.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gehnljbam.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gjwuwclyf.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gwhbmawju.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gblaqtuzt.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/grpeqtlaq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgvydtxu.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glkemmwrx.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwbxpnhu.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsuagckq.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzosrbjy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gijucoxwj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gbjlixtjw.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gelrduiov.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/getucmwkm.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gxskirxja.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/guohzslww.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gihngafsa.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/ggaxozdcl.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gicncpdze.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gztnkscnp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtxvzpzb.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgbcshlq.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyckerth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gflsrdboz.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhvnwnyw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvdekzzn.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdsrlgoy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdtzzocz.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqorlbofy.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkgygwsmt.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdpceixq.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybbqgqsf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklyfanfl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjottvnd.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrglffee.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gmkoxqkbc.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/grlzdises.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfuvrkil.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gozgecfjw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gingtpwmk.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzdtfxky.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjonzizoh.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gbnrhgrxm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbujddis.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gynarlvyl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/glcespkyx.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbddsesy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/glhokmdag.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvtqkqkc.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtzltssl.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqunefun.sHtML


<!-- 参考信息 -->