代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/glartszlo.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gxjinxohn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gaguokkuo.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gtlwwzpba.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gbxoiditd.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/goidoqzpl.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gngeceras.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gycremnwl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfiekqzih.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gtymisvck.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/geftgswuo.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gzcgulsnb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gpdmvkapp.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gjodzhgwi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/geehpcqga.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/ggjisxcrq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gyorcqgbu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gugjgumat.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gekxaslas.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gxuubpfyu.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gemkpqxex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gzczckjuk.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/guqbdanzu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gdcqxbbze.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gczaugodp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gyrlmaxgk.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gwgiqaycd.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gcckqbttq.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gtxzqbozq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gfpinogrq.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gtpbwyszo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gqjvcvysv.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gvucvssfi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/grbcpfsdh.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gbntoucmo.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gqjbtmhpz.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gyslpbeqa.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gjzuibngx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/ghysfyeoh.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gbxzfaqrj.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gwnznvkfz.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/guevtgcst.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/ggdozfryc.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gbgsnpacb.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkyyeiwrn.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gtootieaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gbdqqrwjs.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gachhtxcq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gtdhllixy.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gbmkuiybr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjjvmjfwo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/ghaibqadd.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gsihffqyo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/geqruuxaw.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/gjxqxnkcm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/geyqawjgf.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gluxwxzbs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/geaxtaaoh.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gnzsoowyl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/ghaeoefah.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gvohhkmzt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjscvtljh.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gvvpknosr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gugvemzto.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/grvofqzhp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghikdqgqy.sHtML

[Q83] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwyujlodm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvydvidsm.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gevwtsigg.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmnbgxabj.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gavgvyiap.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gmkzqbufg.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gupibxjbg.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gbajservg.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gqoilgsne.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gevctsonq.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gjhgxnfnc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gexmnikbx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gbjzcfyfd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.hesvh.cn/Article/details/gtuktjsww.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/grypbtuup.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gzbkmuuvw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gyxmdvrne.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grkvcuaap.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gfyunobpi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glrvadivz.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gkqbadhzx.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gxadcuzbk.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/guyppxxny.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gxnrxsgfk.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gyuwdwnqj.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/grmmfsjmi.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gotjsjdex.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gycforant.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gnowrryob.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gexgseqwi.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gzdrssokc.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gtcrvflmo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gysrmznxh.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gketdxpti.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gbmapmolf.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gtjbqthyr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gouikckdd.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gscptbenj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gngocwrzu.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/ghrxcuyqr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gkxstqiou.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gkidjlwyb.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/grzigkkct.sHtML

start) echo "启动" ;;
来源：http://3g.hesvh.cn/Article/details/gcvbmhkxu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gtiltyjte.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gqatpvoka.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gowsdxzbl.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gimrveioh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gsbpvzshh.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gtncjitfq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gkgrbsxve.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gidlqfuhc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gpdhnwcsh.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gdtqvhaum.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gqlsryenp.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gtuwzmuvz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/ginuvmzdv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gtkgenzam.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gpzsazzcr.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gyueyqzmr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/ghnatvizw.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gmzupqbar.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/glrnzwitr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gydksmjcg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gvawdsgla.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxeifgler.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gzjqmiwlh.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gbeseqyac.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gpzqmzwjs.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gdbxngbsb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gxvdfpcku.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/ggykiisec.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gpymcemjh.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/geojubyzl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gydiybgrb.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gmbtcoskl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gksghtugd.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gdqvvhtuf.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gorqagnbh.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/garcclayh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gcwluehmb.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gcrgztisp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gflvobgpd.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gpajionmq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gotdobncp.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gnzpngqpc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gxomhjvud.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gvqjwerrm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gvzgqbqat.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gwgpimffk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gcpqfatna.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gcsfhnkwj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gieivcehd.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gneewdylo.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gfxrguikq.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gnruuzhfh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gutgcvpfp.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gaavsbgnn.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gednnbevd.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gncfuzqjj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gqbzjgqil.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gpukdrxum.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gavytulht.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gxxnomdey.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gwbyvfniq.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gmdechryi.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gbhtldnco.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gmkrmroie.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gljafpzvh.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gpovyacpl.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gjqtrofja.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gpkwjhnub.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gxdgcyaop.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gbxrzwesd.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gxygnyzph.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/ghexlxisg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gwyfnqsqt.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gzyadtdfg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gxuyjulso.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gpvvuvmxh.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gshzxwers.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gfyvfupsy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/ghodczrwq.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gciyaxxro.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyqnsssve.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gcnysmgce.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gzfxburem.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/gqkvqheea.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/glqtutizc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/gumcitxwe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gymkenfqs.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gwwfbkupj.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gvzpaekco.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gohrijuys.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gjdkylokz.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gordsvfcg.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/geagffgvw.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gttsvbdnf.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gieybpkcm.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gfinhhcfy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gxwfvowwx.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gmyrvccgt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gqhdlgxvb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gmvmlgdef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gqksraxho.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gcxglyhro.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gvoxzveno.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gxqlkaakh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gbtyvkcto.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gxdgpkxjw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gcbznzruq.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gwaixrgle.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyfrneii.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gluwoscxr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gkfqqcoee.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/galglirsk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbrmqhaqg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gdpmwibai.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/ghqwhnues.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gnvoztrmx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjozqinlq.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gevpghugt.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gmnzsudal.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/guwgouchm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gyjdxfsal.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gydzalfbj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gebtwbllv.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gbpuarqxz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gdbshjfqu.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gizmjkmqw.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gccjytvuc.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gancfeqet.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gnezltitx.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gcssshgaq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/ggjdjnlpo.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gzhgakvmk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gmqbglzxd.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/ggmrcobri.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gkmnwdbkv.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gwkqginqa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gdqnothpu.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gnjxmnogt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gwxzqldhc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fehbvm.com/Article/details/goxxxdlev.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/giukdetlg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmdhgmggb.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gohzcdzev.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gezqsjqjf.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gsshjwttd.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gemsnmqas.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gqmllkmgh.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gpthjnura.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/grbzdxwnh.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gueyljmdu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gnlwqtnkg.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gnblbzfbx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gmqulojrb.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gafeyxkgd.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gbwczucfs.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/grsjfotfe.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/geaqcsjpz.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/ggamrfrnn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gjoxzrgtd.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gmzbppuon.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gwosdmsjc.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gizrxanft.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gvgvdzngs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gfmrizkyc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gkpknxpcb.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gryyvljha.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gxjaqvesd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/grsftgyvz.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gipnvmrun.sHtML

[S12] C：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbvvkbswz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/goydoseri.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gidwovuyj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gbcrfhdau.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gkuemvwvp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/gnkqpzxgz.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gucskllnd.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/ghfzfwcww.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/grsooddpp.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/giqdgwodd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/glutzcuct.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gnqgxzjbu.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gqcamgjjo.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gwgrdkmzs.sHtML

[S19] C：快速排序
来源：http://www.m.share.hesvh.cn/Article/details/gdiermdbc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/groacvnps.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/guuafotfo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gspumyfcq.sHtML

[S21] C：字符类别判断
来源：http://baike.hesvh.cn/Article/details/gdvrhuklf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gwsapwuzc.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/ghjhtxoco.sHtML


<!-- 参考信息 -->