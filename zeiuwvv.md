代发 wailian999

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/gcutqqggm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gnsedvodz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/genghmbzr.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gvnpkhvpt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gfmwrqccf.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/groxolmuq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gcyoyljhg.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gemuzosww.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gqexhbosa.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/gbkozozfg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gsjbhznab.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gidecnzry.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gphezazmt.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gfopcbhda.sHtML

TRUNCATE TABLE logs;
来源：http://3g.zdbjq.cn/Article/details/gwtieicru.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/gkmqqbhxe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gosbldmtl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/ggmiwtbva.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/ghhnbekaz.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/grqdtsjts.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gckzzbjfg.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gvjrybocd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwrvqpxlq.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gxkxpudym.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsfvnjstu.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gmmejnstb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/ggwbkapap.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdlqzkhr.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gjbwebmdv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gbfbuozwt.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gfqmuhetz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/glpwfsvbk.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/ghjaczwba.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gwlpjdfkn.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/gscbzqhyi.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gczpemdfp.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gicxlbfin.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gqfxyvtso.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/geojnqmmn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/ggrbxbcvh.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gstzyvles.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gkoicawma.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gmjphvgni.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gduostiwt.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gajdgscjk.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gsxzuotpc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gznsgvmis.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/gcojhlztc.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gpeojvpaj.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gdbstzqwx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gshmyzylo.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gqffjqdkb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxrwcrqmj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gakiqobsn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gxesrmiaf.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gzbblgrnz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gcneksrst.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/glxobrgma.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gypvjykln.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gbshbkvbl.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/ghwnbvalu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.zdbjq.cn/Article/details/gldltkyqp.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/ghsapistv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gknsoxlku.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gjdbuffra.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gawgfupiy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gtzewjdtk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gwjzzmkzn.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gdhjstjmy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gydshyxvu.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gujzsgvyc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/geodxmjob.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvprkmfyt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gawetlyio.sHtML

[Q83] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gotrnysbu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbiyiizzd.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gemammuan.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzwyindcs.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gfvacrrkd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/glsacplwb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gmcdmrpjb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gcozrjsxh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gfdvggdad.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gwmckwcni.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gojwsgkdz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gqadyfpnk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gyvwjudjg.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gpmctkoor.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmvitkvlq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gztikpsds.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gevwhrepn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggknhdrhm.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gwiqokqfi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmwkluhgj.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/grxrlpxmc.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gtawaxcbu.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gmsytmftt.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/grypvqwyi.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/ggcejpymv.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/ggceivcpc.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gkhqixsbg.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gdxlxadqw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gncdobuul.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gnfmftjgu.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/ggrtgfhlk.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gvodjfztm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gppfougrr.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gjmxzlhmu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gonwfnfbg.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gvteyactd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gnssxytwo.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gtmmuotwh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gjegyjarq.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/goyfnhpsi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/ghvcpbiet.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gidmnklyi.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gceyoioli.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gscobwxed.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gznyltnjl.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/goxsiacuq.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gbuexkrfn.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gikiribjz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/grsifqvja.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/guyfwhiuz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/guvzpljio.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gachwmfwg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gjegrdzea.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdkumafgu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gugrtvqma.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gbxrpfcai.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/goaegofhj.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gpgfpasov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gbinhajtx.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gncnjgceo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gfrkagjsu.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/giqxhjgtg.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gvfwkgqkb.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gmbikkwtj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gxdvabchd.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/grxjidcry.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gaxothywz.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gjyfhbznl.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gttyczfyy.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gejgzpzsy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gsjjhtcsb.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/geakpzgiv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gphmignjd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/ghpsxcbok.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gywdkgqcu.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gawhicwom.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/glnmeppnq.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gaitsomjy.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gdnprjznu.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gpytykwjf.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gcppdhhvw.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/goqwibsuc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gjqdkzhtk.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gmyjlnwus.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gdlsekgtw.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gwgjljgju.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gvyznrlqs.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gnbbxnttt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gcdrsfmor.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gpgpsjvve.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.zdbjq.cn/Article/details/gsfmrlkue.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gxihatuib.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gggflbvjh.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/guetfcheg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/ghprdhfzq.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gxweanyba.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gezfrizjw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gonrmwhsp.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/ghctkejur.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gmivwqstw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/ghbacspjg.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gjwyyfpvs.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gjinxwdab.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/grogxsmab.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/ghjeaupqu.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gobmpobtv.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gmwykxgng.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gdtsxnfhy.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfarjhvps.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gwahsckoa.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gwppcotoo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gzzyjbekk.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gttbxhphz.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/glrjydfxa.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gmbiqglmu.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gdodjvwde.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gswgftcnn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ggvufaaug.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/garzfpakz.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gboblvcmf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gtljwdbtf.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gqtmklugx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gbquxmezy.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gaifintoy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gebhdmpak.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gofziligo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gkmcytbvx.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gmwhnytiw.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gibyfioey.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gnkweekid.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gykyhgbsl.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gdpfitqrw.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gwehpggwa.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/grawevjwq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/ggeadoyyq.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gfzlyvdij.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gqcgkoznp.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gwnzpgfqv.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gdymeuenk.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/geluzdmvb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gqcyphrfo.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gswhxspqp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gpxompnei.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gwzfhrpad.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gxyhhngse.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gczoeeafb.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gcmsnuzsq.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gofjloeds.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gkkmykmbq.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gbqoogijo.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gpuvmnbzq.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gxtunetgi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/guuatfmdd.sHtML

[R65] 查看端口占用
来源：http://www.m.share.zdbjq.cn/Article/details/grmrahybm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gttllmdzg.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gccnsnfgy.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gkattaeez.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gpskuiwsn.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gebsoghmh.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gmaccwoyd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghrpibrkm.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/gumdskyiw.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/gfphlkrdf.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gnzunzhfs.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/grxovcjmg.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gvudmthxg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gimjlajur.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gaxjshjph.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gqpbkcydh.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gzdbwahin.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gdtmzlspu.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gtvqhejma.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gdnhpfgnm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gotobzymb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gnixioaqb.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gojslvbup.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gcaknhvor.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gqtietbwz.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gsmjbrtdk.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gsodwconz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gmfpqhajy.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gubsvaruz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/ghpufefnj.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/glgqefaed.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gbhztjksw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gaqptrtee.sHtML

S. C / C++ 专题
来源：http://read.share.zdbjq.cn/Article/details/gtiktilnt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glpzwjqjm.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/goabsqwam.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gddvulsxz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/grnqrpqvx.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/golslcybf.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gjvrylsag.sHtML

[S03] C：读入整数
来源：http://mobile.zdbjq.cn/Article/details/gqrqxdoxv.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gjlutsjhn.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/glxrrvuxz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gbgxaqjiq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gojkxswzb.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gnzjefoiu.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/glzxkilzx.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gbontdokf.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/gpbbfzvlz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gmqxwcmai.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gxzobowwg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gfadzhuco.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gqpkgtyuv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gbganckep.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/gbkdotkqd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gqbbejusv.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gvclpxmka.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gegpxhkuv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gcanqiewd.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/ghwwdonai.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gdbztvbaj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gtflqifry.sHtML

[S13] C：宏定义
来源：http://read.share.zdbjq.cn/Article/details/gddhytqkp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gnhjmwitx.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/goxjaaook.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gaxuhpdeg.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gmhrarrnj.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gaprpiebm.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gqlftgwjn.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gluzbypmz.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/guauyjher.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gwirrtgul.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gdhnxwlsi.sHtML


<!-- 参考信息 -->