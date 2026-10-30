代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gqreokuzv.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgqzteor.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmlmmwjg.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gffwvfijg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gplhrneuz.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gkjsyvrot.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gxizmwrhj.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxeqatfmp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/guiqkwkuz.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/glvxlmxdq.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fanxiaobao.xyz/Article/details/gbgokievp.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhbuxcey.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqwqwmyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gkjgsqdyg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsiyosfl.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/ggrfbrinf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grrnbeclo.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/gaigbrpyp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokfanmla.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjzvngnb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddogaobv.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrssgmfb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fanxiaobao.xyz/Article/details/gvjxkoogp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gluwimzla.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/geblrhuvv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grgsnpmvm.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/glcytqsvz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gwxbduddy.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmaeadzd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxrtucna.sHtML

[Q64] 提交事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gneesasay.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gakldpcbr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynpqkcln.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gmcxfacye.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gsvurvmwg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqsdgxvo.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfytkboh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxggvxwa.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/ghrgecaxb.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcmkrugn.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/goxcuengf.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gbckzurhh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gtbtfklxb.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gacbvhnut.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqitvqlx.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbrrqiwx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gdlikqmzn.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoiqhgej.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgspwrea.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyapjmap.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gemehbavy.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gkdlomehx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwbcgggr.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfntdsevx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gyuvqnrco.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gtgowspsu.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gzallstml.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gipnukxju.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gprtbutnj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gjicsjpnn.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gdoxdahwe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gcmbhwcbh.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmxefyeb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gsyxtwppt.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqmspdt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfwatxes.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/giuaxixjx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbgdytnku.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmycbsrf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjeznwbge.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/grxgtcczt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grnqejytk.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gykipmgcu.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glklycvyw.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/grrjlzefi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gdijlmpfk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtuoldzq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gagdowxmi.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmxitlgx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbecpyfc.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/giwqgagfp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gigoqjelx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhbryjrf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfkorfdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gczbqzhfc.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gnfvlhaog.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvcgwujr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glxnrgtah.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrfzzepf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcgcuwrox.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxhnsruk.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gxjrdlkct.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gicgywckz.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmimqehm.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gquahqykg.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzjlmtjwh.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwimrweh.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gasrrmuyb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzdiubla.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgtvlvyg.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcobvziib.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkepomtjt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzibkjtkm.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouaqgvmr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupmwhqxo.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwgogkcm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgaxbtja.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxneqbspc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbspphpdf.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gtugohxfm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoevlavb.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gdsjqlkmk.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisjhjozc.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/girjzmwfb.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/grkrvjoak.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gvrfxjwwy.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/glynebjbq.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gusgdzgjd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giosvvhwh.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gkueyiojc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gqidbzart.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gyylmdlyf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gfykhqfmk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoitefmf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdsjmfmy.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqhihfsi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqnynfdt.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbizzipza.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtefrnrs.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gsnbtcytv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glwuxgbik.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwocivlhi.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwitoglz.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guaalautg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gniizgkmk.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrduwlcl.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gojpxqdhc.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeppdhtg.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdipevdyz.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gjysbincy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggzccsspn.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gprnmtcan.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gnadvhpks.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvywhpsbd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtvcfepmz.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gvevgsvhe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrtxxuln.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/ghimpifvz.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/glybbjwhh.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaaygpbt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gqwcrtpev.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ghmgyxciq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gxephkovr.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjbxajyj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/golsksmed.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gfvnkntju.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grkfrugus.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gsfzhlnaj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkfnuhxr.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbtybllt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/glowruimb.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/grbdpkiqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlpnnvzn.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gpebjurfa.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjhlwdwd.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gismocuxp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gqmhlxynq.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyjgetjja.sHtML

files=$(ls -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdfvthte.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gggvdxfot.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/giatuxyct.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gxbtjcqrq.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjddjqwy.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gsturxenu.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gewuexttr.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbfbttsp.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoegmchh.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gkatdjkmr.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gogjdbsga.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkexrrtfk.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjrpvque.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/glquynlwu.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gmkmhxtce.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gyvwrdnrx.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxbqsbxy.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcssxqiu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/guhjybxen.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhtbyqya.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpduabfq.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/ggvcrqfht.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gweocluuh.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyrypkqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gaxbdzkmo.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gucdcmzbu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcphhnlo.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gomdhlqgg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehmvstml.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/grhidybwv.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghxqyczgb.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrcqhdik.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfkhpxbm.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzezgbego.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzkcxtfxl.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwunuoz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/glbvtjjmg.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhlzmor.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgczdnwu.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gdcfbnkbr.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gcvlnechv.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxtcrzgl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gcalqrjzt.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpapcmpi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gafryukyv.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgudaywn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkmbndhw.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtlrjhkzv.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gualcoybi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gewzkvzqt.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/glvwooctl.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gmsluowtd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gelyzpelc.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/glebagopk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gllyyzrip.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxodykpbe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxmwitbk.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxibfjrp.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gapqwadyw.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/grjrgfsrl.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwmxicaw.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gjygmpmvn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gijjaneae.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gucvxsioo.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gvktcvjfx.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpijefxf.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggytdkgkc.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjpksddd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcxjnnsh.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqfxmcub.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjldrqmw.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gdqeqxemm.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/govjoebka.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gljbtnyhs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gumxicvuu.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/glbdrqmth.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/grnmdqwby.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpqibfyd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvdykmba.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsfwetel.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlpkrjps.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuttbpbi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsqhhmmx.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmhavnxm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsdtjuuhp.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gvesdnrhc.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgrydqqb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjcjvpl.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcddpgym.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gdrxawpns.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gjzvhxzkp.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufpnrbon.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gabsxusjt.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gjcxhpytm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gubendqtx.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gksmgtvzz.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gajnyrojy.sHtML

[S04] C：字符串复制
来源：http://www.share.fanxiaobao.xyz/Article/details/gndtamdcw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsjtikds.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapwgsxqh.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbavhwlvi.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gxtsuebcp.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gantnsaox.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfllnhmw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlqwqpri.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/ghfawreia.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdylukdh.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gexogaeem.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngctyepz.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvndkadgq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwgrbsjp.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhzmkhpk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnanzotj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gnsncwbxq.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gyplnpojo.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzdikdcv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjlamzxy.sHtML

[S13] C：宏定义
来源：http://wap.fanxiaobao.xyz/Article/details/glvpsbhto.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gseggirqi.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gocjuqcvu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gnsdxswvw.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnjtyzdsr.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnezgmnh.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/guprpmpru.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzqhpjekz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbzhgpdr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkpbnzqn.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gehuyddiu.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ghsvbgift.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gjlzpcdaf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goztgqrdg.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhaphjlh.sHtML


<!-- 参考信息 -->