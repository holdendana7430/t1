代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvddinhpb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgaamnzn.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjvxmpaet.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbommmfl.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gzmnzemeh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gffsknjsu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/grvmzlaeu.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrniapdh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/grvfdiwok.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzedcerkx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gazdooudu.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzrmyhdi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqhhzkob.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpuhoedp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/grympjlqn.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gpywtdxsj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gcajajoby.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/ghljbmphk.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjycczht.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gkdoyxujj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gmsqtwdxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/glfaljzie.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjpdpsor.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gqgbyyqeg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpebszdhl.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gxleuqaiy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmosbzfyd.sHtML

[Q59] 分组内累计
来源：http://wap.fanxiaobao.xyz/Article/details/guwfugjxt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpetvkoyy.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisfcdcuq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssbkqgyj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnfizmyd.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeoyemcr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmadyebd.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gczplcckm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhsbrnbq.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlcvphoa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gnajasmxu.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/goibuxfmx.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjlbdvin.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmjolgij.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfgbtlxk.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gwlnzthqs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/giplunpfd.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gtomvncul.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqtpnkh.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/glnvtlpom.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gleufkwpg.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/giyzjwiwc.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/giootcsgx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gmwshdezt.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzszxqrg.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpiwnvsz.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkqqikyg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlkniuwg.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/ghnqejyll.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkewvazil.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gooxiywvd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/giyozqufq.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gkmgpngbh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqjvyybd.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgcmtbxp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwpsdlvde.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/gvrcguqlr.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geudhvglj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbereact.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpntasjpn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnvxzfel.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitovwifs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/goomqeclm.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/glgsbhuno.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gixqxkogr.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxxiafjf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gutdbbgox.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjpeqykn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjszvmzad.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzwifbqx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggqdzvrdf.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gihcojten.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/goasbrkgx.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gatusxaxc.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbsbrrdlh.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gnbppseps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gujfpgahw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpjfvpnr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gvrmmncfa.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gxbgnxsfq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giouzmhhv.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/glgtzairj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/guvdvdxiy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozqunvlu.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gkcmmruiv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnptqppf.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gqwwtuwnw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvmlqgmw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ganlneyvq.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/garaladoo.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gqykpriec.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnrxyuou.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gxikdutst.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusdvrybe.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gyhxclsii.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gbxzpfcwc.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpwsjepb.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gtagtiytx.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwshzamv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdsayxqw.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdcxivyx.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrfjxcrl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdmsoxhc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkzlljwfc.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpsmabjcr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqyoefov.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqahpyamz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdjrnfol.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/guraryyns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxddivbci.sHtML

[R10] 正则匹配
来源：http://3g.fanxiaobao.xyz/Article/details/ggutwmtbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/glbuioghg.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gojrohkcm.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/guyyukwsx.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gehofjypx.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjpmiuqi.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcqqionl.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gdfldqfjn.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzwcgauv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gfeamdfnr.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawhvomag.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwaafyox.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gpznqfaml.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkdlertw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlamkpnx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsvgqpsz.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypgoturh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/giyrkgbji.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gffpjaeue.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbuugxsw.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsykmngo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbqgnjtd.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnziumyfn.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmfolerc.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gvhzkfqfq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gubogjjqu.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gpffsonmi.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqrhltcvs.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqxpojfi.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gnsluaodu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gbwqehbpy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/grjgezipr.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjfhisaml.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbgvnzxhi.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gegmobyan.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gykslpiin.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzsgtwiac.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gupjpdivt.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gmoybljev.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gioxwmlqx.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gtvbaicke.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhngujxk.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gslpclihb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gbhccpvyh.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqxjhge.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/glxajnjge.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwvcoyra.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grfnrdhxq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehxhpmvh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdiunlar.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/ghkgvqkzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gspjszgum.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtolgugv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmzpltmxr.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gocyfufgd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gliqylyrl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxqonzav.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmqelhynf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqtrttvvu.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwopkgaa.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gsguvebdo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwwlkiab.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/giolnybyz.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grezvpbex.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gedwoiwcx.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/grwhvtreg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcaomiziu.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gkpgpstqe.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gopkzdcth.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gndmtlfur.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwkiuovm.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsdfdqid.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmjjpxuyu.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooxgimcf.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/grfynpiwr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/guipljvlj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtarcvnnn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafqfyxua.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gowrfntai.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmtuyckxd.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkrloraj.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyacguvvr.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gskdivyjc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gokukhwei.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gribyzjud.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpeyxjqq.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gbjgojold.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkfmeymf.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeihlumo.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswljsqfx.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gveyswkff.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnazxtogj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaojeyatx.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrglwpzf.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/glfletsli.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyzsksro.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgyeooyx.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/grpknawkx.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtftsspkq.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gznaaqqgb.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnmuazhul.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gxeihxbgz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszzwkaxl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/giccndtij.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gbczbtbvz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxqizolhm.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/guuwwctmp.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gnmgesnpt.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcdtlhyys.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/guiesvxhy.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gmcrfakrr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gaypyxpeq.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvteqklnk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gdqtucmlx.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuuckgfq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/giicxjhux.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gynwgjpjc.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxuwuyurq.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gkflbltpf.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gumzqeqcb.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gswieakph.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gycuuxayp.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gmijxiltp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gsirekvkb.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gtypdydsc.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/grqubuciv.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjimnsdiu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gcdsaohnf.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqrwzkxd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxhaselbr.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjghlwejv.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gceldfbhn.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gzpoekoit.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/grwnighod.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpefhjwue.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcctmmatb.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghbvpmlrk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gypkpgogu.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfvzfsu.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/geplrfexo.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/geidkhhpe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyffopeg.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmzjaqtn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmoogarc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxjstryw.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gozyiqrqt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbohshblb.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/grkyvxlst.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrbvjisj.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwjmowwd.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gebyupzmi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnwxepgfk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/guesjpiiv.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbdeqacg.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjajypqv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gssgzevsd.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/golsehbrz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsliuiuo.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcaulnlgo.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdkgiwki.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxejpuwg.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ganaftwdb.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/giyoyulas.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvzstzwv.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gheakqdgu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnadkeyan.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gtsstzlwm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlcxtwcb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjdhnqqd.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgyiipoo.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcboincx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gtgoddgeb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwvrmlpx.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnmqtbhhx.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/glxdojzca.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gcljfvbkt.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiislrnu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gxeanylpy.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfolgxlp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganxgtode.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmnmkomg.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfrnirwe.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvrbmili.sHtML


<!-- 参考信息 -->