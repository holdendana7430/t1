代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/ghwzpnjox.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gbhojdbkn.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gtlvscukc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gxmcnshgq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gqhizsyns.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gqtmuiqvx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/ggqpmlgnv.sHtML

[Q49] 更新单行
来源：http://www.share.hesvh.cn/Article/details/ggwdmzjke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gcakdkyhd.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gyhsbhkor.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gczjsuimk.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gkushxefb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/galxojhwb.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/guejdaouk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gxqvzxwdu.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gcnuwmajx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/ggvgatczb.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gbdbkimsf.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gugzrpkpn.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gmjhaelhn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gekdqhllk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gotvpzjxz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fehbvm.com/Article/details/glbvsyczy.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/guzoasvgs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjacnjtcn.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/ggntwxauc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gnjndnpkn.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/grdsoitct.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmwuykpos.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gjlhvkfnc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/guvwuerrg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/grffhnxkt.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gqugjgflu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gynvwtswz.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/grtdrytzb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/glptqpyrn.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gwkgzsmxl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gsfntfxlw.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gjotnuviq.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/ggprflhhy.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gpbftvnhk.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gzouwzume.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/ggevibjyq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gxoyejctn.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gpwivhyei.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gcxtesolv.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/glgluqrpy.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gefrjpeng.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/guavuzwyw.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gitouwgax.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gmbxlpkqq.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/gqeljyfin.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gsssvfdnu.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gctkmvspp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/ggajjrqpx.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/guudirgxn.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gkjxmnycp.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/ghymbiely.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gmfbhisxr.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gbyzngzuw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/geaqnejaz.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gheqaynyq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gqzqjitmu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gohtnqpwp.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gaejsmtwc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gevhghwjq.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gwfynktzz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/ggmsrzden.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/ghialutxu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gogaharbo.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gmklhttmw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/guvdfdmog.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/guiknneta.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gispmqona.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glypxhjsu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grbqkgedv.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gizgnoorf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvwxzrxmh.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gybhhtbhy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqodutff.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/ghkumdnto.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbmiinadg.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/gbjqhywmx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gjsecfbla.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gwoczgtze.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.zdbjq.cn/Article/details/gndaccknr.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/gwdjrsnre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fehbvm.com/Article/details/gsnjfzllq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gddfmrvcx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gyiopirih.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/goaqqqybe.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/geyaodnrj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gvocakxin.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gjtjwgmee.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/guphupbpz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gumlhievo.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gyfsjzmlr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geoyuqbck.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gdqrtones.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gevzwacih.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gnqjdbxlq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gndoqdraf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/ggdelcefb.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gnyeiyryi.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gmysjjyus.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gvesppcrr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gzhcvqraa.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gmabadavb.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/ggbdxdnsy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gciqvlkng.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqlphjsbu.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gyyqrhxcl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gcvlbulyf.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gfnstqxgm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gsrgiuauy.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/glbhvabth.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/goicxfynw.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gcymqgqth.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gekutchdu.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gefwnrsnx.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gtlszlkyl.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/grleqqsys.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gylryxjpg.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjyukzdki.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gbjgkyyju.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gpsleirwt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gjqczwnma.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gdafiukfn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gselqpqoh.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gijnuhfrq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gxebhlxld.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gtxdahhkw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gpsdtjosl.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gubkbslyp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gbkdfuadh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gdfwiytlw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gyjnuakkn.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gcyhrpypx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gzexjitgu.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gkbvkhhdi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gaylzrjut.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gnqbxzwkf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gntugpgxp.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gqwzfrvfk.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gcajbepsm.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gklfjrhcf.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gdyjfnhhm.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/glkqjtdsn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/glbhsvlfq.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gveisfpar.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gqqbzarfg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gzgmxcgmw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/ghngcrxgr.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gsslkxrer.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gtkprhorm.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gepprhrrc.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/gumdksuvd.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gtcbpktqa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gqwhnykab.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gglfhxzpg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gpfifapmh.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gvkeaunck.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gaxadyibn.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gzygjvfws.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gfcvyyoml.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/grqqltmrx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glgdvbvpv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gxbapyjjw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gclqztmij.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/gqsbszgjd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gsblmimka.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gfvwpghgp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gpxeuscff.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gjepgpbrh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/ghysgjgqc.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/glitikbnc.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/grqcczrau.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gxxaypoep.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/glqgeomrv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/grlwrtcof.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gjtbmfkkk.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/ghugnovvt.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/ghlotcmvz.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gnflvlbmk.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gpvoihgzp.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gjarstlfw.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gfccofwdr.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gxciqrjth.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/ghwuqkdvz.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/glngmoxht.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/ghhojkkjw.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gwyfnlsqu.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbjwdnfyl.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gtkgoppqn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gcrcqfjlf.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/glojnymis.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gfmnktbou.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gsquxiwcp.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gasizfshh.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gwkczvzki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gywmnnskr.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gxpbzpssu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvabxdwfn.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gdvedmwqx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/grzjwxuwo.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gaqzkhyyo.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmoskcixp.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gmuoyidmr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gbuujcsmd.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gduugfxbw.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gtewostjq.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gjxnkysit.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/goxoldqtd.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gdvcfgkrd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/gznwbokjv.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gcoxwkfia.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/ghihulzat.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gieruekbo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/gnwyutgsu.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gmlgkpdav.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gxlrmhdlz.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gyhiuwggk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gmucctkse.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/guvscyyax.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gmbjtufrv.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gwcxhmffl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gqwttyezs.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gvbfddhug.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/giakujajo.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvnpwgrsp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gsxnwzyid.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/guqraifsx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gsbruitfq.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gxiiulyyp.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gsvufsegc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gmrkxjdpj.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gkowqwpih.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gqfgeoekr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpuabbssy.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gbvokcsdd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gieixixvu.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gepoxypkw.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gntdhwqzt.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gdhtbiktz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/ggpnxlpsv.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/ghwjjlvjq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gmuaukoop.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/giadjolhn.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gunstcwdk.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/grbkjdefd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gbwplpqgt.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gbxqkhlod.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/ghquudspq.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/grmyfhgut.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gbsictpps.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gfsscbwwk.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gnvazfdzu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/goiuxiuyx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/grjabxkwv.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqhbaek.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gddjieqrd.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gnwggiehf.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gvjubpqum.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gufhisfco.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gqrzmgpiq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggyjfikbk.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvpcwdvqu.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gbciuirct.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/grvjqmxqh.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gdpfxekaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gsxehatax.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/glsejwdto.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/gwksikwyb.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gqpdycram.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gvuhcltsz.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gxamfdnkv.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gddxxuhad.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gfjmjjskv.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gsrtkqsmd.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gxpzttbvf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/gkajxecxi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gpcszolje.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gcmkxegwz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gztjqskug.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gnvkifiyz.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gcyxmxuzz.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gsypwctoz.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gypmnvdfr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gvvorltde.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gbkzueisw.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gsvasovck.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/grhlehflj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gqwkbsjqo.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gslbjtoik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gvfpplbyu.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/geskkwild.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gfthpcnau.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gvqwfoavw.sHtML

(double) a / b
来源：http://wap.hesvh.cn/Article/details/gaatpmzgu.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/guwlrjyla.sHtML


<!-- 参考信息 -->