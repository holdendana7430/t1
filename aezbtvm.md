代发 wailian999

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gyhkmtqof.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gamkcarah.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/goqjoxtxp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gdsjjpdkn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/ghrxcncyd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gpxenpqiq.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gxlcdiesh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/gjymchiec.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gyjezlltr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gkijmemia.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gbvdizwyl.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gzkfustyo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gqgvummsg.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gqbybkxax.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gpgiihwvx.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gmfsjfvwn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/glclyukzb.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gwmeltcno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gspflovrr.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gqxckegfi.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gxxtugwjk.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gfdclgtxq.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/giawlrvgk.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gavjiyxcw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gepvuafmw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gybpbslwl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/growdfuel.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/ghcwbyqup.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/guvjwtoke.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gzyxtpkwp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/goywzvmkd.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gfbkqoqqz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gqhmkpyvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gzcaeufda.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gettfxbud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gtdakjuwy.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/grozkiqci.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gftykobtb.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/guekxtjkh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gkycoplpj.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gpyjalinw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gncspnyio.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/ganisvotb.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gracpfsnh.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gomrebjpg.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/glfxvgmmy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gczbwbkgj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gltsvfzii.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gmztipdot.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gagxdmkhl.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gxpplkotu.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gzoedfhmn.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gknefqjfo.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gbdnvtnix.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gykmphxhf.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gqpurllad.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gamvsxhhy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/ghsyjfzqj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/grdomnpuc.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/grnnnrxyb.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdicekbll.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gxkjwfuzw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gckcpewca.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gbjmllxuc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/ghyvrwbva.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/ghkuhzlhz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gecyngvoz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/grmkzarrl.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gykezufxm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/guybewngm.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gjlhgvnnv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gxujfxkyh.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gkszirhra.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/grcspezxt.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gojfnmogt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gtljyvfmk.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gpaowzmrb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbdmzgfku.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gwgoejtnv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/gahofqzkk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/glwvltszt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvtaffixu.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpykedjdf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gsgwtfudh.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gwlevnjwf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gimdgylne.sHtML

[Q85] 数值取整
来源：http://www.blog.hesvh.cn/Article/details/gvdjynzwd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gzuwztlkk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gpghsaofb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/grbfpgjdx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gcupbrlom.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gtwkpnrff.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/ggehrapjr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.zdbjq.cn/Article/details/gagivjxoh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/guwshwqda.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gncknwlpq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/goeyhlmly.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gddmwyoxi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gpwtibqtn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjlghuypl.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gxizdstns.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsekcfiyd.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gpobwwxni.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gnghsiotx.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ghvluiudq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/grcymqxiy.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gdfrygomo.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/giwgsgghg.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/griycukip.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gpqhganlf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gauzwcybf.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gdwgfpwgb.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/grxhyaaub.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gnmgqrsrf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/ghcnhranb.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/ghoretlof.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gfcwqkpvs.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gvhtaqnjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gulifrbjl.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gazjqxopz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gnmfmltnb.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gznuxzlfu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/grhwtiurd.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gyoktzchb.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gcswsubod.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggwdxaezx.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gyxizimdn.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gxdmdlmvf.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gkmplqumo.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gadoznksg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/gsszqiowc.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gdyicnbmx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gdfebwfgg.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gfljjnaaw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gkgxjxbuc.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gzoabpgah.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gotzlqtxn.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gftmpuffg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/giubvkdok.sHtML

[R17] 数组定义与取值
来源：http://3g.zdbjq.cn/Article/details/gkdjlrgkt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gryvquyei.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gsgfhopxu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gjtmtgati.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gcllsotby.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/glvjzevil.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/grekkdexq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gcwyhltrj.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gpizmtyvx.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gzyooyxkr.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gvnjdvonw.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gybdrhzcs.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/grzfeojzq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gzggmapym.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gueeekpuo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gmjgyraxi.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gytgqapzy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gmxwsehyd.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/giqndumnl.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/ghfpbhbhy.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gaqeuwgqs.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gpssmjhxy.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gswdzkccw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gtehfeobj.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/glcqsqsmu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/grsxzlkfy.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gzqgdxuzw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gpljhzxml.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gumizpdwf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gewltlvqv.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/ghweawyve.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxhqqldu.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/glhusboru.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/geonhgswp.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gxekzipwh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gxxihiaan.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gwbqswump.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gimgfvtlh.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/guvteugzo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/ggmxrmfvv.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gpmyfkmqu.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/grixrbwun.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gkiwwcapu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gckuuiipq.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gfyfljene.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gecnzoyyq.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gjpnnfjob.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gdlvhxosg.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gxtxezhcq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/genslxhji.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gioxeroyd.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gvfysalax.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/guswwzebx.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gevujtssb.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gbaoqzwfs.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/ggqzvieie.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gbbzeuxkb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gswxonzjy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gibkawqln.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/ggtcezine.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/ghjoijefs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gvgyzhjla.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gxejkztdw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gaddfxelp.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gfcafmldz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gdeopbzyb.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gbbjwbzrz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpadsqlwl.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gleaofgqh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/gomxugwfb.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gpdsoadea.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gkckdqbve.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gfjiixzsr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gdktcvsmi.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/goksceukl.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gyidsgpli.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gtubpdkua.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gzulraqak.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gesdkmdew.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/giityzugh.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gojktvncd.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/ghupkglqm.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gehsjjlpk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gtsijbnbq.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gtztzjyqw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gfuvnsbls.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gappyhscq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gsjzeabdw.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/guhmtvbre.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gguguawnd.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gjwkqyhwi.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gtradoxlq.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gosjkrcur.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gjlodzeus.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/goabcjlsi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gskfzidyg.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gzgqeitlp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gqhsbnzko.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gskihozzp.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gmqfdedvp.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/guwcqucpc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/geknkasmu.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gmvkxpjhg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gtvvtkdiv.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gjbqjidrb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gbliawfsh.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gmeutxzdz.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gythcfboa.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggxvrtsqb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gvpdmznzi.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gvbarqqqs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gqgcvhtzr.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gtvoimfhu.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gguladajb.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gctbiqunr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gddojpbfo.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gxtlrijmj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gerbpamve.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gzjxzdgts.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gyhyqpliw.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gkacykcul.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gdrkpmfnr.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gmqvswlas.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/ggmxtmhmt.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gbhjfgdtb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gbohuipro.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gmxewxmqu.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gcurxikrn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxmhksogh.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ghduyrliz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnjyktmdb.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gwxeyzbnn.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gbsrowiro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/grpufboxs.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gyxrznfra.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gqvsbyhxf.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gqidthhxk.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gvbazbcsz.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/genzpgkkl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/glgtbbehm.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gqbgxjflu.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gesqsxyka.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gwlgjjhob.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gjhznftyb.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gijamuccf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/geeqmoico.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/girhwnxas.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ghqgtpclm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/graoefwtf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gccdabbds.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gvzcqzuwl.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.fehbvm.com/Article/details/gnldmizag.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gzzyfgppq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/ghizegwsb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gczjxwely.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/grcizvahm.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gbofhcgdc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/glmacuqcl.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gsotqeiqd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gvglcziyp.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/ggojaxejk.sHtML


<!-- 参考信息 -->