代发 wailian999

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gevvaputk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gqghqkdnc.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/goosdrjil.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/ghfluacnn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gcedryyvh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ginnypvgk.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gtmdqbbep.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gwdeckesu.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/gdsyeqctr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gcxhjrkfi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcmsduvj.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/geeopssvu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gjjkokunv.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gkqecckob.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gdnufwejj.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/gtbemoeyr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gkfymcdgr.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gwqtkcgvb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/ggxreizqf.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/gfzftnvlt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gldjzctko.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gyvjrolou.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.hesvh.cn/Article/details/gdlvtlrme.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gdzexicji.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gyzozsmrg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gkdgifhyr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gnxklygar.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gxctziwtk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnlyifsry.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/grjltqvzf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gzunpqqwp.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gyjrdipry.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gljulqyez.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gklhrcjms.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gqxmjwegt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ggwjlqekh.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gkgqqwmpo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gpbblklda.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/guboqhiel.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gfxcopeus.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/ghgeuakpe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gcglyktat.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/garzcvmfh.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/ggzngaltx.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gnxbnddjy.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gyphuhlmj.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/glefskehn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gjcgvpfen.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gdoiesggf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gpdvcodeo.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gavnkyhjf.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gustqebhs.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gagvzzeaq.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gvmhxaywe.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gbwarrzgz.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/grenowtmk.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/grbsztbfm.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gkjwlvqvy.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gylsvwnij.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gockkvuzj.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gzwcxvkfy.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gegaamagc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gcwgqplbx.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gnoidnzwu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/gduszeksp.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gdeqdiace.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gixhpoqhi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gpspewdrx.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/ghmuswxyw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gxpoczstt.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/guuqkydqy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gtolvnycw.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gjmbzlqkz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/grvhrzexo.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/guwnpgtuy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gqrcjadgn.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gilvdpyuq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvaaibrhp.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gnwnfaytl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/grbbzkrhd.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/gawwnhiaz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfiypjjvk.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gsjnlqmoo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwjboevdp.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gtzzcmdvq.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gdvfnvvpa.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gomdavsoq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gpdqmhxpn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gtrrngunv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gfmiyzxsv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gwcsxtaqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gwsfoyyxs.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gmvupklbj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gxvfwiban.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvoajaanq.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/glvddnsim.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/ggtlivnxv.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/giiclgdcm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/grwvbuydh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzxmbfpuw.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/ggiipipnw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gppqjusbd.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gbktosdau.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gxruudgyf.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gutbkdhui.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gqvlmundc.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gybsvqtqq.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gxmasceef.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/ggnurpqld.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gjixsmtvo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gwlqlgwkx.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/guomplako.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gzgwmxdxm.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gzytpgeqk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/ggmraogll.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gbthtlbmd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gntbjlozo.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gywfjpbcr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/glbmyyvpd.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkfksttva.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/ggixgjtgc.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gwviqqebk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gcojhycxe.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/grxcgyhds.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gmkudywqd.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/ganpqcbeg.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gcsdihlao.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gbawfztru.sHtML

esac
来源：http://3g.hesvh.cn/Article/details/gdktmdkqr.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gtghhqszr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gwwcsleec.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gqbzeabqc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gogjaxcgy.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/ggtliahha.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gsqvhiazt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/goukvmmpk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gwdodbsgk.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gfnnxdxwh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gcfpnlfjs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gceugazqb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gdzsjpksc.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gqzzubemk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/godmbspgy.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gmyvqxqjf.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gxrwcxhjm.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gyebnlltt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gvddmmovw.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gclydowev.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gjbzbieza.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gipcdjecs.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/glimdkssq.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gvycusbjb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gfsqkylek.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gupnrfmxl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gxhsyblxp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gsjzmapna.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gblzuisgi.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gqbkadkfp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gausbcooh.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gshqyvwht.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gkhpfpedh.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gntevyhhs.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/giylwfdlu.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gladczfoa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gdynafcjh.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gnpvyatkz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gyktsihtb.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gkqgjhryj.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gruzliipe.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gnuzwcufw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gadazezph.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gdrmfgqqt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gqadggujj.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/goyumnfct.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gubrgugts.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gxpskwqhk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gjwcjubne.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gqenjjgei.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gvvpqiotv.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gqmuvwivc.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gxjicrwoa.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gazvhdbem.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gelhytuzf.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gqbnbrxdv.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/ggktsxibx.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gvuscnzcm.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gtkrwctoe.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gkzgvnrpv.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gstombwnc.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/goerplvko.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gvedtoygx.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gnsggwpom.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gzfwqvxiw.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/ggddmaema.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gboiqjldx.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gcjkaylps.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gqyxsoabv.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gwpbssgnn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gduwzyekf.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gpvfbsneb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gbwgewtoz.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gsbthnype.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gavgbbhgm.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gnmuxzyuj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gisiwxhkq.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gpzztjnkl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gwxswiilf.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gfvyvptor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gimznznrc.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/guyowiuay.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gnwfphvts.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gdnlmmxab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/glsxoeqzr.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gtfgkcqej.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggjqvwkzl.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gqrnemenc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/grtteotvo.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gennahgcv.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/ggkxmxqdi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gbibznzzj.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gmedytpko.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gyfcaskhx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gcepozroz.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/giytqftek.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gclhioelx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gnahdecfx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gmchfqpoq.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gfdrcguws.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/goqcaoaba.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gkbxxkymy.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gyjnhxrhs.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzeoadvke.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gpxvjdsex.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gabwsrtqw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gpklctgcw.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/ggyvvszvp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gcwaminpw.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gtiinpbgz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/govankxiq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gornuwcwr.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gezbyvsau.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/ggkvukgbo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gekqagtfq.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gvhumghfd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gjpwqqowv.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gxfchdwcg.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gvphssmva.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gyqqjbjjp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/glphjpztg.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gftxiepgt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gojdencdx.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/grxvfamiz.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gwzvkgzem.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gxxgnsnyz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.zdbjq.cn/Article/details/gigacexdu.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gnwqftwon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gzamwezmd.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gcczpzbia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gqingjhjc.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gzerefevz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gcptmwxzx.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gxrtobuap.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/gbuduzaej.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/ggjgbizfg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gymvbbobq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gezjobnow.sHtML

time ./run.sh
来源：http://www.m.share.fehbvm.com/Article/details/gwojfjiou.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzjmscskg.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gaydcfusr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxdnstfor.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbebaxotn.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/giafoferw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fehbvm.com/Article/details/gozncznns.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gxdjqzkhl.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gscmtdxat.sHtML

[S03] C：读入整数
来源：http://m.share.hesvh.cn/Article/details/gdeqnohco.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/guikjnnfx.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gztgdspbj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gnkipfasg.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gkywtlkzk.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gxtivmzpv.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gzouzrabf.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gjofjnzxo.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/ghnnbacak.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gnuluiudp.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/giwjtblmz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gwdrdcmxf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpkkeujvb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/guorzeflm.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gszawjzqi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/glijthnse.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gycdmtorc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gkwypfbil.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gptleqvcc.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/glhmgsumf.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/grqvkxotp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/ghiatnhii.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gblhzndvb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gldpikrzb.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gkagmynrz.sHtML


<!-- 参考信息 -->