代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2cbgvfbjt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2segqfgog.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2mujgjhhj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rcbdlcno.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2elcarhkh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2xbajmtsb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2zbyogarv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2ctvvbwgn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cpsjjoyw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wxpiazgj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ikaedyns.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uoflfbjh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2udgicees.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2urerfvik.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kpsmsaqu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vgdgtyok.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yewabbir.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ezuikfjf.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2renkmecr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zzpdrkoh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2iijpbcbo.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2vafgvqnm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kswwijns.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2dooxlxca.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wevrluor.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jucvokts.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2frxihogo.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gfafkjnc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wixwkztq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2irkgxxut.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vtgtjpan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tjqpafre.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2tfpyxdce.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rrhzkgob.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kjjstunr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2fljzjzug.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nlbsubtt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2cfqvucjb.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bwwwbjcj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2pxemfuns.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2cvrzxkmj.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qpsaqqfj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bhjyswqc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nvwkfxxz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2idumnkpu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2zmsgpgcg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ddtidnav.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fwxynswh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wctaezqm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mzjotzig.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2vhbokyuk.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kmlbsioz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xghcmvil.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zqwcuzfc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2jndscony.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zbpszfyn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wjpqmheh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bsnpdseb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2irxssixl.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qyzwfnxi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2spyjqnrr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vjgwxycb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vtrlurnr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fntrbvln.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yvtydyqi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mglfpepr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2whldibci.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yabkhjjj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2fovhwczs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2yappzctz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zswiahmt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2uxbqlmiw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ehyehudm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qtynehhs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hjknqyuv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2unrvfgnn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lxydcvsl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tozwgdvg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2axhilwsc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2inatdmcz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2joqyasog.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lwhfcaut.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2behggoup.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dfzkqtbx.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2aciujmwp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2brulicmq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vphqkqhp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kjuzhkev.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vnmvkglm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2uqzraclq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tbwdbguz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xwljlxjk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qglbcyua.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tgwytuof.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2jvdflzue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcrykbzn.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vjucihha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrhueygl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ukqadrmn.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lemesjxn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2dyfipevh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bxwznqvh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xeghdxpm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2cqsmrrpt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ayybkogf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ebgmrjeq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2heljbdtw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wadiehij.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jwmxbhcs.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cpoilvwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2opdcnnfi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2trrkltan.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vrgbjhhh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mwligtfx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uvckzufj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tlykhlsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nzmzribd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2taugggrb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xmxalckk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2gcbqkute.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2plrjrrmg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kaeambbi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ophgauab.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cykfnyqg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2uikuqbxg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wtuqbmvi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2npcpspdk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tgczyeuq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2abjfiwoo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rxhhzane.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2guekgshb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pvblzxea.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bsifgbzc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wccpsbvn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kgkjkqpl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2abduoopm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwmgdnic.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2nxbbfuyd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vvmnfvhv.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rmabgpto.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nykynvxn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2qdbmrbyf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2nixombmj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mwqvtyrt.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hshxdtmj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2bisnpkrs.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wpqqdsjr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hvgzdngf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2rtpbdkuv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqkxrkuk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgkfdsfk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2haojwoaw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xioixsxv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wniaqikp.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2mzzxtpbp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nfugrutb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yxuwovlk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2zijfftlc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lnyxiyvx.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jgdgulxu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ktvcbctn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hwcfskxl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2boesxjvx.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yczmmizi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzjpagct.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vbriucsr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2drotsvgj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wwdegmxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2hkipfhud.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cutnfmtq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kkqtlrwj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wpndnqyi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mwqpaoch.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bauerfpm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qnqsfisl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zszbvlfb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2shcsnhot.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2kjyotsuw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2bhnmmfva.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2psmsemuk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xzzgwpjf.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2gtdngfec.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ohehuwur.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2pnuspxyu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dcdaivqn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rzttopyf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zavsmgfu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gtnjofwa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yhncqebe.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ypxowjja.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cxetgppt.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fzwmpkqc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dyuvcevc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rrtvsner.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ioexohak.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rlmjjpuh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cofqawsj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yietbzts.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2amholxzu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2opkonbzb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2axctjlnp.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2uwueqhbw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ceebppjz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ciuqyvbj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ursgowdu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2qzmtgfwh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tsxilcpq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ipqmngmd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ncsrsqtl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fbtikdgd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kwfpfbun.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gfopvnzo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yyvqnbpp.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2cmmijwua.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rrptzzoy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2afdqvnwd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dypuybwl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ujeougey.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hfszhbcc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sqnxqqve.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rmfzresz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2stwmfgbp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2mdsvpffd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ngwnklot.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2lpkklckc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cyebgfah.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cmwrlrhd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dconitue.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2mbhomyfv.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zkphfcro.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2myxdrjgq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2givmwfmc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tcrcoskg.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ocojwxnp.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vecbosan.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kcfsbhdv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tdceausu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2hkdohztd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kofejkho.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ttmashtn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2imzcpvlk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hfnupqfv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tbviuurl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xqarlmfs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cbbrhxmi.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2vrdofaea.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2krdwmexv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2josznbor.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2btxpxqyw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2epxxtbys.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xnpgxdef.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ylkznyup.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2xxskezga.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwtkhgxa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zfgylmui.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ugxhsiqk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2jehwvkyl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2rrkkuxxu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2viwjgwli.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2biaezczn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ihrvpqgg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qndkdouf.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vialtplm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymwgiqbf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hewtgaxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdkszajj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kgwksojg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jappwuix.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cielbapj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mvykvmzs.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wxsshkoq.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2mrqajmpv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hjzyaxxr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hythshot.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fjwihpkw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgyfkqxb.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jeyylqxw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dhtiysqf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2tmutrlep.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2yoydrwqq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2aiuymgxz.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2umtmoqrk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2venldynx.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mqljvmjs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ntkfnfan.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2pnvmingx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2rgiusbsw.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2avdcxmhd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2xdbrbjwa.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2heeiloqp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ldtifick.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yofzxena.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nlzxvkkf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ctvyrpgf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wreodkfu.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2gditvyuk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2skkgddvo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jakabttb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2sgujvkqz.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2hbxeauly.html


<!-- 参考信息 -->