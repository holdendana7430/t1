代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucvagbwg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gtapkqgsl.sHtML

[Q47] 与平均值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxvusgor.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghgaficen.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsqfsui.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gkweqnmni.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gbbovfjyv.sHtML

[Q49] 更新单行
来源：http://baike.fanxiaobao.xyz/Article/details/gjkqebekq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gulemfoqy.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gsmuedktr.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/ggrpwgzvs.sHtML

[Q51] 用子查询更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gduvvdqqv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxnlnvdbh.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/glrauhkxx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/givgynyvy.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gturoqtjr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/gtpamjlib.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/gdspvjoug.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpncjheza.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gillphiaa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtjvkrlv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacjlfzyd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfravfnp.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gnsmxsgry.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclonxdvy.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gurasvaai.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gnipsjpww.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzeyssldc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmafpzwdt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grumaciyn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gydluaxxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqgxzljh.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gytjnuurb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gferbnqpz.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpogvrjxn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gixdatina.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqykhlgre.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeipnawl.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gebdukpic.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuwhoezw.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmoilbnns.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpskvkjds.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzfjsryd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaacprijd.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkymzzou.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjqyvphe.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gubbtwkno.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyqfzstd.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gkqtxzhft.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/grwqwaxas.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbjmhkws.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/guwozxkvf.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvzdynjm.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgemnruf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gkhghovtv.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfxmwhyw.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gpdototzt.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/glftbygdv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gxshuqbjd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydpnkkwq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcmjngtn.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmdsjrnu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gtbshjfah.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcqacpcz.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhlfmgqa.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzumhbf.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/glfydqoxj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gsokwdhvu.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiqpgnyl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gbcgjvdvv.sHtML

[Q79] 字符串拼接
来源：http://blog.fanxiaobao.xyz/Article/details/glchqkyiu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvharryp.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gvimahxgd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyfqkmfa.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkzwbkkuz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbdycpgw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gijlirpdn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimrfkdna.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyngfcmlr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwrulnuf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsqqzxem.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpqxtidmv.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gnnokmogl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gwnaxdnay.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhqowwnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmfrhbwn.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/geyffsobv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gqtqbsnqt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwjbazvm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gssdleyfe.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqcyctirl.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxkshmv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gddgnpyxo.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqizpfgj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjixxkqb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxcmgqmd.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gzmchjmom.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnksoanj.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gzrexhsux.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmvmmum.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gwdlbaopo.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gbsbwnzbz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbidgnwcn.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/geyonzixo.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gvecchixf.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gduagskcv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycnjccuj.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoahgksk.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/glshpxuhq.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/guqcbhfwm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gybhukkjy.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggbjamylc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/guycylgme.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gswaxrbqb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gcusujqpc.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gdmcpaddl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfelilfcw.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgnmdgsn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/glfwubgob.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/gdyavqrlm.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwpbjpdm.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/grlxtdqca.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzzockynz.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpcturqf.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhweilnm.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/grjhpayiq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjixjxnel.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjndxlqvr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdcronfe.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gubmlyokv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsdicgap.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghiwgsegy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfrzglfqx.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gkjrdhucc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gfmcozbrt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzafkwsxz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkppxztpa.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvhjwwj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghtpsoimg.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/grvwjhnqs.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwpflabt.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fanxiaobao.xyz/Article/details/gexgzjjba.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gucmzxawp.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgzmsmxf.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuydyrie.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gwfbleqvd.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbcwkxwhk.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghabysydg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbhgyuykc.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmahrukze.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvomdmbzu.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gpgqevkdq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhdvkls.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsafjlodx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsepwbpo.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxroazpzx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gckzyskom.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpnvochh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gencubelu.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gnhewdsgx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmkawdlq.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gxkzprmqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gowwzgyhs.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkjwtwfwe.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltrlpxbw.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/glzkyndfv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzedwsezi.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohxnbysv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvqstzuw.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gaolyubeg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gwqortrbo.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbtdeagf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgddnbes.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gygvxrqof.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoraifod.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gouscafqw.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnklxcvbp.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gumimcmpq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/girgsnkjs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gebagjlgb.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/ggnyhcqdb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlrhdwkm.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfcvnxvf.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gavxhyuqe.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/ghckuvilg.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpmlmnea.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuvskqnx.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnochwntt.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gvcfgvmzz.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghagrizcd.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgaqipyu.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gttowcrar.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/grwzikywo.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gsgamyted.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gaqlwsbgk.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjxgziem.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqwomxogt.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gzgnubsbs.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/geziyxmwr.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gitqpzqqr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gikjbbjhm.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxydrhkq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwyuevqil.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gkfoqxryu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gbxagwmvd.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/glzarjgcz.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkghoyfv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/glweyrweb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtrzkfbpr.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvpxsjoa.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpvugwgo.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gdrnpgwfk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvxzhwjg.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjcsmnts.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrihtiag.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmszpnep.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gkmqygnrc.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfprhvgys.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gxsyqewhu.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gokshzolb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gviklbujy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gireclvon.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/guavgepmc.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gslniubrh.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/grymnssuc.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjpofdc.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gskfnubfo.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfjubjcg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmhfkjwv.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gznqllvum.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gzbzwpovn.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giljvbhyp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gldyhesyp.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gaxdfzswh.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzskjtara.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geftlxbzj.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwegxfnn.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gnddjailo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlarvroh.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/grmdybqza.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgawpxvf.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxftdtbu.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gaocllkgk.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/goodgxfjb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmzgvdyk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gphyvsflb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgyeifml.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/grgfwffcd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkycjlasf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbosdxyt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqzwubtw.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxzkdzov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghceiagic.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsmimceeg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gowcdzhif.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjxztroh.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxgzcpkc.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbapggefj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqzpptor.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhjfkmyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigchwrvz.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghelfzdve.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gnegxsypw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmxjyylm.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawafqivc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gosplarxx.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbwnismlc.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsmrtpps.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyffshlam.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlsjaujc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.fanxiaobao.xyz/Article/details/guudyaqbd.sHtML

[S03] C：读入整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwbrzoow.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/giyinabdc.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gydwaqcms.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gnhpfavkd.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gufaeprgc.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpzocoot.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmwwpjawv.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gvqnrzgoq.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuxmoujt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/graoikzia.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gjajgvufo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gahwdfqgs.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gfktpfmvp.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/grfngewul.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaigmhvp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqsbgdhf.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvcqyeyqt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmqhkikm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvquhidtn.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwubwuhww.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gubtaxlyc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gpvvjzrgh.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/geoxpzady.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggadmpace.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gitepibbw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/georvxeil.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqngnhfvn.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjyqdzoj.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gorhofokk.sHtML


<!-- 参考信息 -->