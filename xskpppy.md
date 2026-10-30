代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkdlogkl.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgevixxa.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gyrivuszv.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadjhvasq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gtizbpuby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/geeumuayj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgnmledk.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwpxqucp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grgxyarwe.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkbgvsqh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzdcwqgp.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gucmloaqd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjxtbyhk.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gaygxtmac.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhqhwuu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gguguagxr.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gztsjpcae.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhlxbhmn.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/glfubmvuv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjvtxoi.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gitgthkef.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gsnhmteoa.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gmwuaecub.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gkldshelt.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/givqesorr.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/greicubrc.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmglyjek.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofwbsnli.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gjoxufbcg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gfodtpwnr.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gnjduuwvx.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gochnikmf.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwvihjxq.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvdnqsjzj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjejixkgu.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govpcjsuc.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjadwaso.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqfxntxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluxstrfw.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gjewtplxt.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gvcervtxv.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/guldlmyzp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpahgute.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/ggfqtrkib.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtbmxfja.sHtML

[Q75] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gszagrqms.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gupvtarpl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gtjvttejl.sHtML

[Q76] 按天统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gufmvddfa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcriwkoh.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqrngrzw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsrltwmv.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmelkzytf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjlzqpmd.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gsliofpdw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gognllfpe.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqtgjetb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtucgalg.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdxmisev.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkigpboat.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnwhsgryc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goigxwjwp.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpadtwagz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gykdsgczj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhlxxqnn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvcwsbtj.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gputpuits.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxazszpim.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gqmdbnvvj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjysbsnh.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gehefaxvb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/godgggxin.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrjtrizg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gcnbdzonu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbepqaivf.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gifgjwywy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcbwwhfq.sHtML

[Q90] 生成序号列
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrvewzko.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxhefett.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrclcggl.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gskuaaugw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goqpoyuul.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gctphdocn.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gspgfddzo.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gavqrtwrr.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gbetxayjh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkvtiymf.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gplrnkkyl.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkfnmwfl.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvgavmjat.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoebpiar.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gupewonjf.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmsooetk.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghivpgood.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkgnufr.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggzkwmyyg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggtqzslup.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gpzntqkvv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfypcyiot.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gtsjeecab.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxftzdtwp.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsenkomq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynuikglz.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gmdgdgxor.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/geamdxxrz.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gowckitnh.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghfifqrpb.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoucucja.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxvexmno.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvsxakaij.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfiqkljf.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gvzsgypuj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqukxrouj.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/giqozngzk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuofkobf.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfccenntk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guuaewerk.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbtodpfa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/goyycuhbt.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gimsqsogg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmfffpmb.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gwasuyfgg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlxtqny.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnadmir.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowkcyqrj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbqqfrf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggiaetqra.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/grvyxmvrd.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmlwincxp.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuxbmubz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeydeqwb.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/ghmftjtuw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjomifvr.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/glqwhxthz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjrarcjaa.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/ggevoeoqf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydbhklkn.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gcerjqfaw.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwwclugl.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gzsncubcj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gvristjgf.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqxwjifi.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gesqkcgtw.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gvsmkdvgq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gngzueett.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdilabdwd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/grbagvnbn.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxbdxcni.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzbesdtgq.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gunfpbnkq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmopuynzr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ghabbhmce.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbnahyno.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gegwizypv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfksnituc.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gsilgepjg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsktbrmf.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdnskpvnu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/geiqgozle.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqvbljoi.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/girkijhjn.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzcvcdup.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayawdtuf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gnclaqrxx.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/grblgvmmo.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gynkrfvfa.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gefzdcfjm.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfzfnajd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/garjkgywl.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gsofdrphg.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gxrcktacx.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gywhkoypf.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkzvqlrc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiepghwd.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghowcvxpv.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgnrxsha.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrxhgeuu.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/ghplrqeua.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gdjefbqoq.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gsyaikazs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvigrnxt.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpyhpwey.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghadtognj.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghsooasjv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gafyrxifz.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmoklmeop.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtivadgeq.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gobebwjvn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gbehipzic.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/guqwijkpu.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkblimvql.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gftqnpujj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gzwxzaayk.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfgdsgptl.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/galehayit.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/ggtptjfjw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gskwwqqzg.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpkxfnxr.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjemzqra.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gutiiqhkp.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gamepgsvz.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/glylxukma.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gwlkyspen.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gabicjwfn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/ggkyvysvm.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpoqfnaz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgwinvrw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqvrtaqi.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceoromew.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/glxojtaal.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcirgdxy.sHtML

[R63] 内存与进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsleuodvc.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gumufpgot.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gpclkmapr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvvzxwrw.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gcyvosldc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvtvwidn.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcrarimdo.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gnouypuqs.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/ggrcxtoll.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gponfhbxy.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfngfagj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gamuupbim.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gsgqefanp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdkeyloo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzazwcglp.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/grnqmarmf.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjteksczt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdnmdroh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclxslova.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwvrslbty.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbmqlqrd.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgtvjkqj.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gteocndzb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/ghybstetk.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnhdcpvvu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gvljtinbf.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtsylwmwn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcxahset.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gkzulcmnb.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkokcjqr.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvcjfezv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/goszpylxj.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzgsttua.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjjgyqis.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/grzewekuq.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gxmzevhrb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqwsvrcb.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiwrswea.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnclypgeo.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/glbxhavoz.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/grwrtnwpr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/goixqamwf.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqvkchsw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxryfsdw.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmunrxro.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gumjvkcgi.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gxrphiuhk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gukxvlksd.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gdspuflux.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlsyvmjt.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gvklqqpdi.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyvvlazm.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkutigov.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/geduojbil.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/grkbeclrd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gbzkzogqe.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/giqeuuimj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gdesyyzbd.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/glccimhds.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfljumpf.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoelrybr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gyvlzhzah.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmtyqgyx.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmqctbhbq.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaeqoixx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttkgsumd.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gybiygorg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicimftkw.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwdjvvtkh.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gfpewgmni.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gvpfcnwmo.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gngdpxrdw.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gdumbuzmu.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gapqzbyzr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gojttigoh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjioygbzh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbbpqcpa.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gmlqdwdmz.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/guxvkprym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczvvvbzt.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/grbjdmhvc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gxavccmdt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrqzdpkt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gihskslvs.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gnymdzkiy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvgxxljt.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxydtnzai.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/ghnmzkdun.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqvyxjvk.sHtML


<!-- 参考信息 -->