代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ginjthimc.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gbwvzakoy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gpizdxpya.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/goqmfvyva.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmwrohjkd.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gzzatokcc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/grcplxgpi.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gowtvsatw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gusrjpltx.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gtasbbwxa.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gxpgiivfd.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gllkupkzr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfkzihfdd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gayhpojof.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gcvachgiy.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gvtikdnff.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/glgxewplp.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/ghjvvzfvh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzqqwatav.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gwcpaaggj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gbhkgflnb.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/ggmsbvdfr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gclhbpaar.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gvbhyrmbu.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gszauchkh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gkplcaxwe.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gjydilhmq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/guufwslya.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/guaxjtntp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/genwxlbex.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/goyzgtzvc.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gwepybqtg.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/ggfrloopc.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gjbwabzod.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gwaklmkcw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/glyflstkd.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/giktqxldj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gcwsgymzj.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/ghywxfchf.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gfizuenpr.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gudxylwmm.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gwrqsoeoq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gdpimirki.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gcovlaakz.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gulrsigin.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/ggdnthzof.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gphomocel.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gqfuuehzw.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gwxyprbdz.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gdsvcwvxg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gyfqajiub.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gittpwgkf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gairpeano.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gtqmzwclr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtezovbdt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gokzejkhs.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gnjdscskx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gxfmhsngh.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/ghcdsayja.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.hesvh.cn/Article/details/gtanuerfb.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gwaiqmbhz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/goegucqhc.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gfvavqnsr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/ghroxydbz.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gjmghhmkx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gslkbgkqs.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/geerkbyvo.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbxyrrkrf.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/geirdfqys.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtszazkzi.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/glxovkklh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/glxcxtdsl.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gdxhalpxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gizacpmis.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gmncluhyw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gmdyrlgxm.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gebrenqtd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gijwputtc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gbganawxy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gfbhymdmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gagquweno.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/geswmdwnv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gufrumebr.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/grbppolbx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/grnfhhxpr.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gjijjjwjq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gunaswpba.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geurfzyya.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gpnpukiyo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmqpdvccc.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/grwcfapvk.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gmodgxhwx.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gvimwbrcy.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gooanboaf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gxsrxlyxv.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gghqujcxz.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gvfctipdg.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/grypopvlo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/grcgqrndd.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gqnudzkdn.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gpekynjyb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gsapoqrue.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gxguiktth.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/ggrwlbxwm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gwuroafge.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gwyuhryls.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gkblhxfxj.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gnubtmeay.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gzcszdacb.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gjfbfhkia.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gppikyqwj.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gpljounii.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gzoibqxot.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/glrmnbvtb.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/guxryzgfb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gcitdsajf.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/geywkgrna.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gjkabnzil.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gyhinpgty.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/galldxvqf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gudooexpq.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/geaygpwyr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gmkxybbah.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gtvsjvmie.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwtnyknoz.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gdxqxulgv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gwfwdhyqj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ghnqizukp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gbluenpdu.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/giflrmcjp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gevomxqms.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gwxgjfnkv.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/ghfqwofwi.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gmiqddzxa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gdbamhxra.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/ghlyzasqi.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/geqklyzhm.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gifxdokxe.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/guhrquwmf.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gxbpgyrck.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gupredkco.sHtML

[R24] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gbotnmfzt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gmakljylw.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/ghimiwbpq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/glvlxfoen.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gluouijdx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gwoeoudgb.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gfgpicjsj.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gcuxrwxmd.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/ghjyxuxvw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gvndezxbq.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gdpptbedg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gkipqvceh.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gwabaxvdb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gffdmxjwi.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gomsrgrkz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/glnitvqvv.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gnnhoyysp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gjzhksruv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gynyluwuc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/grzgqsceo.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/ggogbjiyr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gzoahsbul.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gjwvpfssc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gungywlbv.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gsfwvzqrg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gkowsifba.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gdlaxhyjh.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gakirxoei.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/ggxygrsid.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gfejwbjbm.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gzmetehzk.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gneadjvjo.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gtmdtfwhw.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gvvxhwico.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gsfxnsstt.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gpnxelqqk.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/ggvuohitb.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gjjpstxhf.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gfikwndjz.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gnnutnvfv.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gowfxklrz.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gfimbdbdi.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/glllmgkmj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gjcptbvhb.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gwzlyibuz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gdmtakitg.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gziglnayx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gwkbzdhhr.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gmcacqayq.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwfiwqfzb.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gstqgbvdo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gxrsxhjjz.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gwpztmuus.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfaugtnqd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/ggbtpvnjm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gxrujwdhe.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gdznwxccj.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gefevgwmv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gspbwgovk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gicexpoeo.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gbjpbtbqt.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gduqsfalf.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gmvknnzfi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gtlllguqz.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gpknvetcl.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gokjjqeen.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gqqyspkcn.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gmriglpxy.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gjhqplvez.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gsdhrxhyu.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gkphkdbxg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/ghhotukws.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ggwpninwq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gkgdzjkbi.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gwsljfrsh.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gerahzfyh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/ghmvxkzvo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gkjucodqc.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gxapzmunf.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gmakrmvnw.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/grxyjoxwq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfcfdxtee.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gtomntybj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gqeuxitud.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gacsadypw.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gfkmvnifj.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gcylbykdm.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gwpowsydo.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gurdkiwie.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gslpqoeqw.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gcmituoux.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gvifenghr.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gaakrjsqo.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gamdflydz.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gazmgzefu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/glnmaixdb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gtffquauu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gdvxvwweo.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gomazmonj.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/goydoabwp.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/gultpyqlx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gtflbomhw.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gfrinfsak.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gazawchqz.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gomgsiztw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/ghtfipjww.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gfnnnauxh.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gjmwoawdj.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gwkahcpuk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/gekhjynbq.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gmyxiwmyb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gygdtlkaz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gpxfhojws.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gdviruplb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjctwnuyh.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gtquauxom.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjhszajos.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjypqefnh.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gjtfycfcx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gxkzofbrl.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/goxyfozcs.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.zdbjq.cn/Article/details/gkvbecsdj.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gjtgqmdts.sHtML

int x; scanf("%d", &x);
来源：http://baike.fehbvm.com/Article/details/ghbvrltwn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gaevoljma.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gblwgkxcw.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gfivklffu.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gjsfninga.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gxmsxkwzw.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/galezkgoh.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gniaqxgsy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gryoxtpyz.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gofmikuaf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gxmrewiac.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/gvyigjjdv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gvvrhmttj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gnahmyajx.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/glzlrysqa.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gmmcpihue.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fehbvm.com/Article/details/gqsjlhsyf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gxedzlqhy.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gnqhtwyrd.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gjjwscaew.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/ghppkuhkt.sHtML

[S13] C：宏定义
来源：http://www.blog.zdbjq.cn/Article/details/gpymvzows.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gvxoiscko.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gcgrzwuic.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/grnyxgtjz.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gtfjzltwf.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gybxdhntw.sHtML

[S16] C：位操作置位
来源：http://www.share.fehbvm.com/Article/details/gyohjhxfs.sHtML

x |= (1 << 3);
来源：http://read.share.hesvh.cn/Article/details/gdbjkffjn.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gunnmcsuk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/gxxdxunkz.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gkljqkvif.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/glnnuwrzt.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gvvnxuyzk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghzqzxhnu.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gzfyeqyye.sHtML


<!-- 参考信息 -->