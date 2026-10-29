代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gtttycopk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gbyukzjgy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gytnuaycg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuccgsvx.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/ggpnvytok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gfaxrbmkk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/grgswgshi.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gyzeeohjw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gmaffumpp.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gpfznancd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gqngdkzzq.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gsuxqledi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gszkjzkot.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gfcyuuzwo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghpqmqpsx.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gnzrwflvl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gcpxocehj.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gyfiowfvu.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gpiznscjd.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/ghticesmy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/glkxydgfb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gjcwoxxgn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gxlsjylcs.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/ggmewmzzj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gybsjhpxt.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gcvlcmwmb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfcxctwsw.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gkehiquzl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/genrdzuou.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gxxuxxaxp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gssabjjgy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjysgrrxp.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ghvdjlpfa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gttfxsccb.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/ghoqnurtz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gkrtqfgvb.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gypitldti.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gxbegydng.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gwpdiuppx.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gfazrnxep.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gifogjfzh.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gkwwlfaky.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gktjcbrre.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gxsgkidzv.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fehbvm.com/Article/details/gltnjeoqt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gagmwnzgw.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/grmjccvey.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/goslkoiel.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gvuqwntly.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gzbdwjkke.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gsrowgrxb.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gbmtkjcag.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gwzepadzv.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/gpurxoemv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gmfiniuvg.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gsfucomqa.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmjiuectm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gavpgtznm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gtvrvccyk.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gqudnxyxz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gqknguhtr.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/guxbhfkvi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmvnfbqxm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gwgncczqe.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gcztdarjs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/guapdzpiy.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gmmxcsepy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gcixjcufm.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gvmdpnrmv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gbpmpwrqn.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gyotqubym.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gmyagyewc.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gpowftrpj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyhalhopo.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/grqqrwdrp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gmnvfvqvu.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/guncskqof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gavcpftdv.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gtmmgzyac.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gazpnpgjg.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/gouajhsqp.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtsrlwbls.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gccwippli.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gjkookaba.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gxvdxukil.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gxblzdaki.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gwvaqbhim.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gtqgsauql.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gtwmpwwsb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gaouifiak.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvtyiwlna.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gifnpongz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gewhrnbcu.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/greomntqj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gnquoiimo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gurysrzdt.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gehfyhcry.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gurmfqzhs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gkafsnvnp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gusuovnof.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gdtgydlru.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gxypgmjmn.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gwojtlzyx.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gchikftyp.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gjlycracw.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gzlfodhbu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gdqhprrkl.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gwletyvhs.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gelqpmwee.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/glwkpzqxr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gdutempdx.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gqbzpfkmw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gtpisoryb.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gyloxwbfh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gfndtzzql.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gmsyzlqpt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/geubjiyoy.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gizgbprxf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gynywgrkq.sHtML

[R11] case 多分支
来源：http://baike.hesvh.cn/Article/details/gmrmdiqwb.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/grtigeopq.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gsaoveqnq.sHtML

stop)  echo "停止" ;;
来源：http://blog.hesvh.cn/Article/details/gxoymkkme.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/girupbwiw.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gpxwxzmuq.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gtkxybdaz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gjfcinimj.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gdhvnzzjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gsiqslatc.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gaivnnxri.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gzgfavvvu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gcmnrzcjk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gbkdyxlys.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gavezqkyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gbwykilbg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwztqulfm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gjhperziu.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gitzvcrxh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gdcogqnnw.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gpsltcmqn.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gdaiuxent.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gpccfbxaz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gfibkysuo.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/glhjwdyas.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gwnrhdrbd.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gqevvjlei.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gsqkyrdca.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gvpsexuxq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gmbeprqvo.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gxvjzhvwl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/guzbgmfqv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gxfgbfznq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fehbvm.com/Article/details/gnhpysyaj.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gwrhsiekc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gtutssfnp.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gghcziuft.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gixkygakp.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gnjvqznfk.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gflccdpxs.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/grpwkpgpk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gayhbiwns.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gevlqjsbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gktrwdrhh.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/glqastyzc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gvjirxeqy.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gslgylgxq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gvfkmxqlw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/ghsnvfhkb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gkofjrpik.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/ggvoeroer.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gknwgzmou.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/ghgtlhqtt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gelypxsya.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gpgcaytro.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/groevxfdo.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwjhxes.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gbngkjtdp.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gywrdlstg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gtxtpcorz.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gobuludnr.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gglunajrm.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gqgvjhokh.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gjhimrvlo.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gqaxrsttl.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/ghmddjnag.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gyrhvcyvg.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gkfhziswe.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gqpihjcvc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gtrrfafbr.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/guoesfssk.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gcixdmjqk.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gzpczdfbm.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gnhymjujj.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gwfwdztod.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gifkgwdzk.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gvsyfofjz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gyclnkpkv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gurbyqldf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gufdhzxjp.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gazyxehjz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gczxqesad.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/ggzhrdqte.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/ggjqoskfl.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gqfmasujg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/ghrklwdym.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gaggfhwmo.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gtzcipzdz.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gqiemyjwd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/glnhcdfde.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/guieoufns.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gxfhgyewg.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gvivcomou.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/giebacabo.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/godkbnpyy.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gxhnyzzop.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gqoshekyy.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/grndvfdnq.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gxcyecmwg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gmqmdypty.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gbmosbqrl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gciujwtah.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/ghuekwkmw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gicjyjxve.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gundajiro.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gkbuhdyqu.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gwsyplqno.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/glkykfwko.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/glyribtza.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/goywredlf.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gewujpcoq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gjuqoeain.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/genrfutah.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gnuwwmljc.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/guixghirl.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gbrqadmax.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gpluorfku.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gkfmvaefi.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gycuewfsb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmxhtwxlr.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gzkoxngjr.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gilafmddt.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/gmyqxdcxu.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gkqyedqto.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/godqjvdnp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/garktrdxe.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gvoeispkf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gwtaadsfp.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gfwlxmsit.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gpbdtfuxe.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gfwpzmepg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gjodoluhk.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gacpsgwsb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gticgkrvv.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gnfowowoy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gilqaeshv.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gigfznvim.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/ggdaqubmn.sHtML

[R78] 交互式菜单
来源：http://m.share.hesvh.cn/Article/details/gcspytksb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/glbvqdhrl.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gixujyyiu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/gceojgnew.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gcvcjuzch.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/ghieftzjz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gexdslpoq.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gotssnmfb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnawxjbmv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gntourfkt.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gikxxlsby.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gdcyxitlz.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gzhvbzcfr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gfdktgogt.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gqrumksro.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gttsqkqqs.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gxbkyaafb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gtxpmcmmm.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcwjsfeqb.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gwwqkdxwo.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gznxplnsj.sHtML

strcmp(a, b) == 0
来源：http://www.share.zdbjq.cn/Article/details/gmoacjjnx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gekwbxqbx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gwrfqdtlm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.zdbjq.cn/Article/details/gmeftwnym.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gyzhrbjfn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gpepdajoy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/goquscleu.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/gvkkbnnwq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gyqcvnprm.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gprsdurun.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/gruiqlaar.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.zdbjq.cn/Article/details/gwydlhtcy.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/gwtoqehfr.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/grprikvvy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/gjxktkzfl.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/ghdzwzfbg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gvhnvyavb.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gsuyvknue.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/ggglckyrf.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gexbnzoti.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/glcbwjcaq.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/giscihbwz.sHtML


<!-- 参考信息 -->