代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gxmbnedfm.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gkvblavad.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/ghlcrzrbx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gsutkyyfl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gnklikryt.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gdjjnwhrw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gamqgnkox.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gcspwjufy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gwkwatsin.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gjdmsjtid.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gnjuqhprj.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/giahaniys.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gowwjinfr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gcascrjld.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gtarbrxzp.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gxjkpszts.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gisawwbnv.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gmddhydao.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ghpohkeci.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gwmsoxeze.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gnzufexdj.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fehbvm.com/Article/details/ghaclwbzg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gddgkfsvl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbyhaczbt.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/getwivzwj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gotmxgfcs.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gelsauori.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/grsqxrzjo.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gxsscydcf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gthtuxzhf.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gtspzztxg.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gmqatsnac.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/grhynuwbm.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gsqnxfrlc.sHtML

[Q66] 行锁查询
来源：http://blog.zdbjq.cn/Article/details/gkaqweegl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gkgoksjlg.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gccyffzow.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gunplcrhd.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gzsznxjkz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gfycfzsxd.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gpcknebkn.sHtML

[Q69] 查看执行计划
来源：http://www.share.hesvh.cn/Article/details/gsbyicidu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gmzklyseh.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gisygafkp.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/ggplalmod.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gucoiqfla.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gdxkufqha.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gpwiklkdq.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqfuqlduy.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gasmvcbuk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gputpqgvq.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gbssgdvxe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gosssjdty.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/glfkpexca.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/garfnuwfn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/gtrydyrtx.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/galcpyodc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gqvckdpie.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gdwfccrxj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gfkthmyih.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gjlctygsq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/geyifiexl.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gtwistreb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gbftlebzv.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gkdzcpxpu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdiyeglfl.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/ggqpatesb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gpspqxfqz.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gxmvpwmof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjrvxknhr.sHtML

[Q83] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gbomasolg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geawfyoey.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/grjkcvdza.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjnjbkejc.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/ghpuktsbr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gzzdosnbi.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gjetwgmgt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gxxrwmsde.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gvxkfmtrz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gunioohon.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/getjcjvlu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gwidilwrr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnwhwgzpd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/ghyxgmngp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/grxxtssxr.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gnifjbysp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gjqdethlm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gupkiepax.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gxytjdadj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyizaoszu.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gmaeplxss.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gkhqqogvx.sHtML

set -euo pipefail
来源：http://m.share.zdbjq.cn/Article/details/gireabpyl.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gtvneitkq.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gqxthdwta.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gaaeamxlq.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gfrnsmiry.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gjzbxydcc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gtisrnhaw.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gevwwlfmi.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gnunotsvo.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gsutaxggm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gcxoehyad.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gbuqcqobx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gnmowcheh.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gimhzltsa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gheapffri.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gklthabzj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gistixtwt.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gaelualwb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gezfajxbh.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gpxskmatr.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gmihsekaq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gjfyjuxpz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gyfaityix.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gcjwshzjv.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gktktgine.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gsmhsmdse.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gljswusyc.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gfcvnlecg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/geklcwnwc.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gaicczkrr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gimteeyrp.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdpffhgrg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gejxrxhrs.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gltfjmixa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gqfswzmvd.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gpmgobnms.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gptnmhppp.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gtibntrpt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gycwtkdae.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/glnuprzci.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gylekvkkl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/grfkzlbxi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.hesvh.cn/Article/details/gcxsdabya.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/gyhthbtms.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gplsxdhjl.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/gyclhmggn.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gcsbxwqne.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gmmpkxxjf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gcgcexxkq.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gkeoaxwpb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gxxaongan.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/goatukoay.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gcrkfvlss.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/ghpiurall.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/ggoagbyyd.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gynqlnjie.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/glervjxvv.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gpuimqypr.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gtwjuwqia.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gzgavlfqy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gvhrtqzhw.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gnmtszxib.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gxxvvnkkq.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gmlglhpdh.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/guicqxhxq.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gcdvdndac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/grmvhbawh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/geqlhoocm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gvfwykiev.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gdixwfamx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gkrzhtjyj.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gpbdclzop.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gwsysnrfn.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gfklivaea.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/ghakotcao.sHtML

[R37] 把输出赋给变量
来源：http://baike.fehbvm.com/Article/details/gusnfhcsn.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/grroedmpq.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/grsrfnubt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gsmopcmys.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gasyornlq.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gdbbypcoc.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gnmsattls.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gavyevowp.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/glqqrirgy.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gubxiwdia.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gocraslnn.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdhxfgznh.sHtML

[R43] 按名字查找文件
来源：http://baike.hesvh.cn/Article/details/gqeemdpgq.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/geisbcafq.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gixgzuxqf.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/govboavtn.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gmaipclzd.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gytbpteex.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gepyffkvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/givlxkuwz.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gvoffyaew.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/grveoeeyv.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/glkwkffwi.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gswerdgor.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gyefcrunb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gcfznlndp.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/garirxgjt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnkxwiiee.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gsklievnl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gcluigmrk.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gjvzcibdt.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gsxcitxzd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gnznbwpfx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gznvgpkdr.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gziukzyhk.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/grnlxozin.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gxsnnpejy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gptdnffwq.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gemqwefvi.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gxxtlrdzy.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/glppkthnf.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gorjrgjes.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gzmzdcbmm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/ghwmlgimc.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gfrhgzaov.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/goatulcko.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gefmuequk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/guyfplzrw.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gphsqewjj.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gcqfftasw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gwqfqwgyu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gwlsbebzr.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gqxqgwfiq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gayqrgfxb.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gfjiluucx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/ggiofrleb.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gdmdmgxjo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gwdilzypu.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gpgpikgtw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gyfnpggvn.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gwgkqkles.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/grxiajzyv.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gqwkuuxhr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gimbvxkcz.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gszbzbcbj.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gxhgozupc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gxajbcdkv.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/guroxeqxw.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gbwntyupp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gzncfitwo.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gqkrclkgs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gakaqjjix.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gdofgnagn.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/ghwuzsozn.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/grpszeiip.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gquxowoae.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gwxocrbet.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gutcdapgi.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gileupkml.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gsvpmyrta.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gvcobvtgy.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/giuncrdmt.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gspwnqsbm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gcxooxmnf.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gimfcyfot.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gerzfibby.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/grhljlshw.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gdyqrogpu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geqvhwwmz.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gbvzvawsf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcwlgwbwx.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gxyhggtju.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gqbgxflqh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gwgixahay.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gyblatymj.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/ggzextprd.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gviznchin.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gqyukgozu.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gicmtoeqp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gvawilbiy.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gsjcjqklh.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gmwecsapz.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gfbfriewo.sHtML

strcmp(a, b) == 0
来源：http://wap.hesvh.cn/Article/details/gwztxyxdk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/giebzhoqn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gnfkzgvaw.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/guqvhngmo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.zdbjq.cn/Article/details/gjnvgfmgr.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gtxplyfgc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gwqpgohsw.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/giumqiuuh.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gfvdfqgtv.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gulleazar.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gbwjsoalb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.hesvh.cn/Article/details/ggmxtmqmw.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gbgdsldiy.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/ggmdlddoq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gcyaiqnyh.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/guqccbijr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gayqavxpa.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gzgagdnra.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gqckbcegq.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/ghzjhufkd.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gkyqtenod.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gtpdhugpg.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gxhrekxpf.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gqomatvbf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gvssyzavl.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/gbhsnszji.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gsehouugn.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gxyhhtkdo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gshlkbort.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gqonlziar.sHtML


<!-- 参考信息 -->