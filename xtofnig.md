代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwtelagf.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/guljefpbi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/glywztcny.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gyebnvsdp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnltxalfc.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gzonbmrbh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gmpcelcrv.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gvovprqrx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gvouecwdc.sHtML

[Q54] 清空表
来源：http://m.share.fanxiaobao.xyz/Article/details/gephaxfot.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmionbvl.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gestkywdc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gqomhnqag.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gumxgfwxu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjbgdjkm.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gblxjppbd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkudhktjq.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gxgctlbiy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghbvhnygs.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/goxoabpmm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gitiotwzp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzfvkhjc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gbklrbxxn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgcbniee.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrwbrex.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwaiwzchh.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gdiwyczer.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/givldbndj.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gyutkvjza.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhaqbeez.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gfhilymnk.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrmanwzk.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/ghdbsbxie.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmjzgciq.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gnfmdbcxh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gnuaqteel.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/grorohrzx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gnzwnhtyr.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gzspcasoq.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmfknirat.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkqucvhv.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gcacgbvhx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstwfoxus.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gtfvfivup.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkahecdl.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gwnjhzhkb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gyokolgra.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/grvnkdhha.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbefjynzw.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gomfdijqd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatcfgiay.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkoregjo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gncsfrvox.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffbbizc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfjgmmrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gatvmrloa.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gsecjvchv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gixyfwynv.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/grnfmqtkw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gktbbjzku.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbdaeipt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbyljslu.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbgqsuqe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/guofwbodm.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpzywtcj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gojbvfzbw.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gglhnkhwq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gpqjeipez.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqbzndnm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcbuuglr.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gougopgli.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwrdmbnu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gofonrqtx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzogmlsc.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gailocmdh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gefnwtbof.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/glpwtwdfa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkiuhcdj.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlixetap.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxpxgmrq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrnarvoh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqtswhus.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grixvgfup.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjobjjv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaopljlq.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gexuhxsqt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwnfxodx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnnlwojz.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gevyrcnuo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpqlpaude.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/glrpnfuzu.sHtML

#!/usr/bin/env bash
来源：http://wap.fanxiaobao.xyz/Article/details/gchkkczhi.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gxooyewfb.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gbakvmzvy.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/geaffumst.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtyeaczpz.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpvnykce.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvsgqngre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gqughrugt.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gizufnxjw.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdgsiqun.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkdhejnrc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgrivcbz.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtonpevat.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gusoihgfo.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/ggvrptqck.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxqlwcedd.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gyduhawaz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gaexoakrp.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/grfgwlkjt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbiheddoc.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gslucxwut.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrdcizkw.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugqyvwum.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogfvurta.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdovljiar.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gnvikqfzr.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gzgzttiqc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmxqhhz.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gaofictss.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbdfyqcdb.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gekwwamki.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gigqemctj.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghtugwnme.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggwitgkso.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gonwqspfa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gleybscpf.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gslhbkfkh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdillatsr.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrswxagu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjkcsftp.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gptrulmje.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzozsxhvh.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gxztledqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzilagdgu.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gopkhinpk.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkugtnqtr.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gnsbkhswt.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbztbhzzq.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gurtqrrsm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwyswore.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhciphrl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjagwayox.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gzenlbflv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmupintbr.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghncrhlzk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbshkdjgy.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgmcuira.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswoefztw.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyeqcwmq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoclvcxm.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrsjrhyf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdbgfudwl.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqqvxtyb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/ggyuweedo.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjvsxhms.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpgxesto.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gszsdexzv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjnxtaisv.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gymgdrpfg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdwkvzvw.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gmaxvytqq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrdvfdcc.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gluxjefaz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsemwtmer.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gawshaybw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrbkidaz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbnmcczh.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcxpjauw.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gcylvdetr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzuanrzb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gxczaezio.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gfikfkdje.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/grxuwhbdx.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlyogcex.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnelgewx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjwvfdsf.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfrwnyled.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guvxisahi.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gutoqzcmk.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gsbxamfbj.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gwwgglkna.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbzpbawt.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxhyciot.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gwvoynupf.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gjabyudhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/galipwxcf.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/grlguurzr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicvefrug.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gywezlazn.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjrqgyqxf.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gfqqvdgzk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgudzxri.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gmfynltzy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwqqkhmgn.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gnoljvkms.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbgssodg.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/glaappary.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpihcvbss.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gntfckjbq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmskiufho.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsnplmme.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gobvpxjjd.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/ggopcxwjz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpxihkpd.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/geukyicom.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgthjtnx.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/goqkjhnpm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrgialee.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuetatup.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsuyljowz.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gmdlrsppi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvuahblf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunshuntf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjefcanu.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/glvrkkxda.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/goxorpyiy.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gsucifwef.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gdmaehiqx.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gsxgwlogp.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gopnuddwm.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gumqdmzrw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjboguycl.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcrfgnrc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjufxffv.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwrqffgy.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfjpvdxj.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gvgacrsov.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnjjdpiv.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ghjeemnho.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruudptlg.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiiksshx.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gnixskaws.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhcxdoyq.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbqfybmi.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlckltdw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmeeybzs.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqjumsot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/geywrsxpt.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfqeiigqa.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/goghrvafh.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gdonawuzi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzcyxenx.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnddtbtb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gijcxkuxd.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/giusafjtj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvblbxvk.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/guvottdia.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqyphspk.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gamlbsxpd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/giauqujee.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gxionvzaa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gterdbpod.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gbpasjqmv.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gzhqyblnr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmsyybgc.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/givxfnuvn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbseyqder.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpthfivug.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtifyjbf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjjfueavi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmjcyjey.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljteizf.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgwvswbz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gccslqcze.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gyfrjrhic.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/guaeyneni.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpkrmuyp.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gviycvjbn.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/guzeaefwg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxgjbyqh.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqgwtjqjg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifdhxemc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guanmtijt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gxvateguz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmbrovup.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gabcihhcd.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdactmgdx.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtavffqdj.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggfbhhith.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvngncyi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/guerealja.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnursdov.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwoxqpdm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggptqumj.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkljuszw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfkpryro.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ghunlespb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzqhnllj.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdaemeit.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhrbicry.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzlnvqhd.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnacttqsp.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gggcmpyof.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gogcyrsyj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgjntfvh.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbhqrevq.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grlrulpdg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gplsnlylf.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/gmvlvrugr.sHtML


<!-- 参考信息 -->