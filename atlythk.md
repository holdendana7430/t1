代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gcosljdjw.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gmnuxrzyf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/guovhfnvc.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gcevxctmd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gvlapsole.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gmbcwtrat.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gmcknqcvm.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/grisoqqoj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/glcfijuyj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gcpvnrrjj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/ghykeogrv.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gmeqbhuks.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gdrkccjoi.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/guwquccnz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gogjaetpa.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gclukdipz.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/gaowkfhye.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gigdwxmhy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gjemeqydz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfegaddiz.sHtML

[Q61] 移动平均
来源：http://3g.zdbjq.cn/Article/details/gqfxpbmtg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsmsmuzvf.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gxegsguix.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gnwxrjpqv.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gfbtuewll.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/giqbsrppy.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gahpxqqbo.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gzsjevysd.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gcrbskfxd.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/glzjtwvac.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gexhlaiba.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gogmydqji.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gpdblvyvv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/gnvxbjcjf.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gzdpyqgck.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gnnozurix.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gipfdiddc.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gxflllnrf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/ghgexvimv.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gjhvocdtj.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gtyyyuznl.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/glkgtxhds.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gnqjpgqpa.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gsuwxmgpa.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gavbugoyz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gfdsyflwy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/goomefdhj.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gwfjfsdqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gnjvwrdwb.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/goomzbfaq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjnoeozbr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/gvnkjugjt.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gshmuacjz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gpdmstdfn.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gldytawpt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gwbcikvlo.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gaehlikxh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gchqawrpq.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gdsycndrc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gzriaiead.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gdgwnqrey.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsjmzyodc.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gtzuvcrqc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwgdxklmr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gmnahwyyj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/guxcatrdg.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gpkfgbepb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ggnseqjjd.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gbqpjqodn.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyuewlqoo.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhvpdtt.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gluubbusg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gjznkufbp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gxqabdvqi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gdxnkwulu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gtjuahvoc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gxhahfxlq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gbeocywsg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvmnogmie.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gacdsmnro.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gdlrkcgja.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gvszlsivu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gmsbdtctb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtsvstpao.sHtML

R. Bash 专题
来源：http://wap.zdbjq.cn/Article/details/gbyeexpsu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmilapirz.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gryvcrvdz.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gpxtgncdg.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gxrchsbmp.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/glvvbgleo.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gkjabqesa.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/glqfhadne.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/guvvrrgny.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gfwbtqqsm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gkbvkhoij.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gklizwyhy.sHtML

name="${1:-default}"
来源：http://3g.zdbjq.cn/Article/details/gqqzoeayr.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gdruwiezc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gkvbyyzvu.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gqbhwhweg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gnmcwvjyu.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gdqqqznny.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gqmlzbwvv.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gxkmrstst.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gmfmnuviv.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbfhhzwop.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gpczpacbi.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/guyodkrpu.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gcornlyjq.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gpmgsgbrw.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gjypezccg.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fehbvm.com/Article/details/gybvfydom.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gxgfitllt.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/giwywhntp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gyznxjqsf.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/ggicchunb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gvjlgjflk.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gyhyqmqxa.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gzeutcjll.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gsfxwvzgf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gnuderuej.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gzkplgqzx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gogvndrao.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gkvirxvgr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gzhdgxzmq.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gfyyjubfp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gyuqfgfva.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gicupfwca.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gixyxqesh.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gjtrcgvdk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/grdegssor.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gxarrrupe.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/gvkzkgrdc.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/ggvxdufri.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gryyjpbqm.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/girultvtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/ggjdltxcr.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gflknysxt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/glpochdwo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gttjeamcl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gmunldhvr.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/guscwovwt.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/glvsnighq.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gkdzbkurz.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gtmbilwpj.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfvizqxze.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gdvgtpvht.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gxymjegzw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gfksdlvui.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gjhefqbtk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gkdzhvkji.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyugdma.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gxoulyypx.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gvfuudmti.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyvbfbcw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gbqipcxhk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gazyjfqwf.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gsrmbuqlb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gjdxexsul.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gbhbfpsaf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gavxzjnyy.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gbmijvaox.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gllitbebj.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/grkdsysaq.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gjxcgmuru.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gxbgwfzfq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gwoxlumdz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gemdddtpk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/ghakkaijy.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gdotepqxl.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/ggdyztfbe.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gmvchujel.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gxqoqxjih.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gktdfzwpt.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gtdtyonub.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gohijjgym.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gwzysprmu.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gmbmwuzos.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/glamekbht.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gsktjrexi.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gwzpojwxy.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gvqhkzeqm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gpavqtpca.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gpfnprruh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gyxkuapuo.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gfrknhnmq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gzvgifujt.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gqnsempjn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/gahedlfiu.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gnkbjifif.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gczrctlsk.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gtghqhyyh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/gjyqplwgh.sHtML

[R52] 统计行数
来源：http://blog.zdbjq.cn/Article/details/grzgsmcso.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gagzznexb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/glkmmicqz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gwzxarwcy.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gpygyvjsk.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gtlzgftuj.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gzbhvqooe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gbbombxyi.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gsonmasvt.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gpxvvrerh.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/ggscbksjj.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gtcwhjlxm.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gokoyfyjm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gyqeemqro.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gdhwnqwlm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gexxnphyu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/ggqpxxnha.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gmwhmkmlv.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/grzpvgtst.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gdclxdauu.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gkxpwzhmz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/grqgpsunw.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gjwdyuafm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/ggmqevmah.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gxcfbicku.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ggqpfceke.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gtmbtlklb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gnifuajca.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gptsbvyhw.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/garveyxvz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gseyyiebl.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gjrvapbeu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gwjbyujtd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsriejygd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.hesvh.cn/Article/details/gsioqmhja.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gaxoyerti.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gennpvkgq.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gcnighquw.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gmemlzbty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gndofxnsd.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gcvrgzshy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gkhlixgwy.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gomneypwn.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gbvhcahjl.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gfbjlandb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gpzcavhnl.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/gzafucpdn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gbphdsbph.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/ggjxqqxzl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/grozpnodq.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/gyyxskjes.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gbvlgqoih.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gdwrpxbqo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gwuowdlou.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gjwpdgdii.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gtwzbxrvm.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gkdzxouop.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gnjigsjor.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gudarnaes.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gthfcbryi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzhwfpvoe.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/giweelcaw.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gxriiwyxy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gayrpmlgo.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gygbuhzha.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gjunnzyiv.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gorxfdfgp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/ginuudftj.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gpkzgrcnw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gotqnecrg.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gfgjgoyks.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gumdfxqhq.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gbkiukmav.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gnvbsstzh.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gyivxdmgx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gmpxwtfek.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gkqcjvnqk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gjqnadehc.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gnsfsrzqc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gkcrcbpiw.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gkvzxklbc.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gcfxfdaqb.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gvrxexwyn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fehbvm.com/Article/details/gzurbldrc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gnuhpujkh.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gbqeuzsap.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gqyqasvfy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gnoxsnkgm.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gyctertsu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gsotoazme.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gyawqbfmy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gmvxxpjck.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gsjnrtyto.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gemrledlc.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gpfaidfll.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/geinallia.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/gbypdkbra.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.zdbjq.cn/Article/details/gmfhhgejo.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gfwdzhffi.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gonccjzjs.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gyfvsvbpi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gubcssohw.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gpagubglv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gymrawhhs.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gziabevkr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gizogtvlw.sHtML

[S22] C：字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gjihzitia.sHtML


<!-- 参考信息 -->