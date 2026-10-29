代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gekktlumr.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/ghcjctlww.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gyipvpyqc.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gbzlbkujb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjkfzzwxc.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/ghipmoexn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gldvmzbig.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/gxyyegxcp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gqvwixabk.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gyedcdgnn.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gzevrsivr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/geqfvatkw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gevdxvrfz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/glhzrozpm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gphvrbhxu.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/giflxqalz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gobrrtsqk.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gcqpalbnw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gvvnoinwh.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gnmcxgkyl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gvnwsyyup.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gnxpsvuul.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/gxryejumg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzkruwkam.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gjtbjnupz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gbpfvmypm.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/ggnpuekax.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwydumdy.sHtML

[Q63] 开启事务
来源：http://www.share.fehbvm.com/Article/details/gsufhdjln.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/getyiazlc.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/guggskchk.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gwccosybl.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gusprmmam.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gmjctdyvk.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/ghecrlzdu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/giusmrayl.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gznabhrnq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gsyitfdzi.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gaqyseuqz.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gkrwjwvpj.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gbcmgncii.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gocnpaykv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/glscvzspj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gsisswdin.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gabxaabwq.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gylbjnthx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/gneuftqum.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gkbtapawj.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gffwmljrl.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/grrimynni.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gsewejffq.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gamiwjjwx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gwjzraenu.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/ggnozmlfd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gulzgweix.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gvrnewtur.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gauqhpfon.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gepqsrfht.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/ggnrkjvyi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gfdhbequb.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gbzanxhgr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gvlqgtkvs.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gycldhzql.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gqqinkbbs.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gvhcamqdc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjiezxgmz.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gyhrukqta.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/golfnnkjw.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gwirxmtmb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/ggvpdfpqe.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gjbwfkpcg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/geuvxltlk.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gstndjnnh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaxyfwthd.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gwyokkmde.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gxrlxdebb.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/gahpfcoka.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gmqyrpdlj.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fehbvm.com/Article/details/gejgyyqps.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/geznfibnx.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gbwlgmtow.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gjtqwmqdx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gibbelcfl.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gzeaoslrr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/ghqttyvtk.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gagzpxone.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gitdmplwv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glmtdtshj.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/guduhxiya.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzrzjcsoy.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gzaqocrpl.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gkvwkcmef.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gvdhcmgwn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gmagpdmei.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gvuiuakoj.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gqtdxunkl.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/ghgycenea.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gzedphscl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gtqoxlnit.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gmalldwyj.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gsvpvknqb.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gcrvuskbf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gndjcbtms.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gwfswlimk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/grpptyyiq.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gbdalxfqu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcqrzgbba.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gcfyrliax.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/geiddcnko.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/grdmncjsb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gygzuogxx.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gxrxenoml.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gglhvkkrg.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gexlxzjxj.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gzdzzeikb.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gfqoeddzt.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gdfcicegi.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/ghzovdmzb.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/guieoedzs.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghbpxmmcq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/grgrhkogo.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gaxfruzlw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/glitkdfnl.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gkpnxosdy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/goduvbisc.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gotgfeeoy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/goyqvnfrp.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gfhiwkysk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gujjynafb.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gxdkzhxcb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gmclypgdj.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gavfrvcte.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gfaoxsmnl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gcvwbyoqe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/galqunfgv.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gtjspohwn.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gdqwwtyak.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gkqfcpqtp.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gyhntljqo.sHtML

[R23] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghzqabual.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gyspstycc.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnbvavpbn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/ggjiomwps.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/ggsknwstb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gcstzxhsv.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/gvasnskai.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gpkeuzwft.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/ghtirkuqa.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gninlaydv.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gqrjonqse.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gzsxzoeib.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmioopfxf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gytyxanhe.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gboziogyz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gbhhhzsyq.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gbspamjwn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/guufllcac.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gfcsfwrvu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gfgkiwerj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gbyydwcuu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/grhcgxtec.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gjrffnwtt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gdiuiuaed.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gtofccsvw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gvwyfahsd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gwxhoysht.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gopebjjnx.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/guwogornx.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gyehmzydw.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gdoasowqu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/glucclawn.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gbsvioxyq.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gfupbqimj.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/glrgxmnmt.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/ghcutjxxs.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/garialgbr.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gjkzpjtqu.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gvhfdzhhz.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/givvqrooc.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gqhtexnws.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gjvfrrjat.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/geqgwluog.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gfqgozbta.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gugcdmjjm.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gblfijldv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gpvjzhevz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gnrvukcrm.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gixdghmoa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gzdyuvvxn.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gswffkhmz.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gebscshch.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gcvzxgper.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gfkpxqbov.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gibbbvjbh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gdvjiuulq.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gkzhnzbrv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gduxmasdr.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gnjclzwfo.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gdsqravla.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gzlbmssip.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/grxsanrtj.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gqsklsufb.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtagrvxsb.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gdwqfgfds.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/ghrssuyxt.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gbbxrtunl.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gwvtqfjlc.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gxxmvsuyt.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/giouopgbi.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gaohlsvgb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gdmcfjyxm.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/geabfxfrk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gboqvqakr.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gunfodfkb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gkjblntjv.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gpztptbtw.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gegtmbwts.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gcyhhdfds.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gehfrcwgd.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gtafqlsio.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gaivfrsgi.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gomcsrted.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gostxuzat.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gfhytuikl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gfhmtotsr.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gahabmzic.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/glrizbgwz.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gqmeavdcj.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gspqaqibc.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gxqtdcnqy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gpnxngqxc.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/glykpqlzf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gfesyduuu.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gzuyrhlvn.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gadqyjmjs.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gfjtblhyi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gwecyyxuw.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gmqiqkdqh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gdciwtezn.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gqwalljhu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/ggrtocvaz.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/grzbmipal.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gciuistvn.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/geefgvsyg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gjhferkak.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gpnxsqfpd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gphbzpega.sHtML

[R77] 读取用户输入
来源：http://baike.zdbjq.cn/Article/details/gyhucqgbf.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gjebfgnhn.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gmkearkjd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/glcpzxbrj.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/gkszqaoyv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gvkmtyslo.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/grcizbptp.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gzbwgzyki.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkiwxlxqj.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gvnkscicl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcdhhngwi.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gxiudpfpl.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gajoyqtec.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gikqxyowc.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/grbezssno.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gfmriungt.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gdsekonso.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gtpmioved.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/gnkobtezz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gzpyoggcd.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/grrcmmujo.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gfunpvtny.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gkvpxbfaz.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.zdbjq.cn/Article/details/gcwydndgq.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gtjgtfzka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gtduexykf.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gmjxbsacx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gmclgxypp.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gorwcpisk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gmlijkrtv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gxarcdsgr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/gqcchwbyn.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gbmoixdbf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/ghnovzwlm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gegwmvnay.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gptqeadtr.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/gwepshupp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gdtawhkvb.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gppoaeksn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gcpisqekh.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gsbyqyyba.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.hesvh.cn/Article/details/grgbaudct.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gpotqyxme.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gzherjedb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gfkidvgtz.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gmgnyzmqb.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjtgydpwa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gyqrelgho.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gythdypzc.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gjvdhawfu.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gbqbwwdet.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gcdqodtwg.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gyatwocvf.sHtML


<!-- 参考信息 -->