代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gjzomjbga.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gvclfwvbj.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/glpfbjifx.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gbdwdbeje.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gozezmyjd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gvratzhbo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gcgzsbsam.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/giyssddre.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gztjnwmez.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gijnjzoaf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqwqiszvh.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gjzrzrghj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwylmqygc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gufixyeax.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gbdckdfem.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gdbzfrgmq.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gshtwqoqq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glusxweop.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gozwchuwc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gmimnowwn.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gwoysdami.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/geohzqfvn.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/grejooaeu.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gesocwybf.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gpquoobpr.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gndeeydud.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gxsgrfgfu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gvjeyxtdp.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gatriliww.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gwawjbygy.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/giriqabho.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/grlnlrqji.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gaxbiadcj.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gokgqunmw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gsxrkubgk.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gsrfwvgmq.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gcdtdjpmc.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/geacwjtou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gyyqszznr.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/goxyaykly.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gvqhvxdla.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gumaivggv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gmjtckged.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/grxzqgrkk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/ggshcpgsy.sHtML

[Q75] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gnzivopwt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkesapock.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/glqayarsf.sHtML

[Q76] 按天统计
来源：http://mobile.hesvh.cn/Article/details/gyftuvjqq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/glvurczey.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gcfnmbbrx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/ghyunlhpr.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gbwthkkaa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gchkiorqv.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gcpqewnhs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gwjzijkby.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gugrmepmp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbwjunfnz.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gzksyrotp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gkjztxyhk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gwnrdwbof.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqlckmcol.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/ggugzerbp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gezlyprag.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gdxppesao.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/grwgimscg.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/govnazqcp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gzhjvytnf.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gusddgyis.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/goxsrwldo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/givvvnuyr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gzleftorv.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gmzbdllod.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fehbvm.com/Article/details/gcovquhxc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwffajyld.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/gubusdzns.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gtyrnpymf.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/glwwqsxvj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gdzulizfj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnwlnelmd.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/ghczyxmji.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gejbcnzuj.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gtkakmyqt.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gogswjjwu.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gahoihrvg.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gnmvlcmqo.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gzdiwidys.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/gkbusddez.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/grtnpffnf.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gzyjmedbe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gcjvtrsbu.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gpxtcgdzg.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gzyvogdmg.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/ghwxvvclb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/ggdwfuoda.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/ghdyipksd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gealmtcrh.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gqluutoso.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxzlfqrea.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/ggyxwnuvf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gbekzyqse.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghdwdtrhl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/guikcchog.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gjvzovyvy.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/glrfcqosc.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/goccvjcgp.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gpnhexjlg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gdizznmcy.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gdbsnirza.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/ghasvmdma.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gmlqfdiag.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/ghpwbozmo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gdiddddmm.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gicpuavvp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/ghswdqlkm.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggkwrztov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gxsiviocg.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/ghbhznnuq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gufwkypxz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gdpdbydct.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gomyjagmx.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gmzthtjkq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdhjbkedp.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/guxzjycbe.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/guzpazvwf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gfuoferaa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gxayrluwl.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/grcwiquey.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/ghyzfnrsv.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gfykxflax.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/glbpzbklw.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/glzvdeial.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/goolrfnvj.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/ggcknrtpx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/giffmowxu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gswpvntrg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gmxmtpqtr.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gwywwtayi.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gcpeaafot.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gkutfpyqn.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/ghvdnwpbq.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/gpieyjpyw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gkqkzvmto.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gasxjvceq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gbekrzval.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gcradilzm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gdqytnwsu.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gmiqcrutt.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gsxzzjigr.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/grxzzntyv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdxjhbhd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/grlbnroks.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gfkmecldy.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gpfvaikba.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gehwauzxn.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gdqxbgmya.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/geaexnxxe.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gtxebiogo.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gmykeggzr.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/guvqzmwtx.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gmyxjyvrj.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/ghtbuggpr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/giksudizd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/grvddvanp.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gknscwxeg.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gficdzeqj.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gdbvlytnl.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gbmqujbqx.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gublybobu.sHtML

[R42] 输入重定向
来源：http://wap.zdbjq.cn/Article/details/gqfwuaruq.sHtML

wc -l < a.txt
来源：http://baike.zdbjq.cn/Article/details/gnuymubng.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gvnostglb.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fehbvm.com/Article/details/gsfuupkiy.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gcmnqpeid.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/glwvwwilz.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gczcllnid.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gvvejtgcz.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gycpghnav.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/guqtrlmje.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gsssqugnb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gbvqeyzfh.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gfkrvwkmy.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/glxugxmpq.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gknywrhci.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gdrkthdcs.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gekhwsjvk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gskpgyhgs.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/grinxabel.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gboozihzp.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gbwdwstgd.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/ghacajymy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gllvypxkj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gujzygxgy.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/ggkwjyfts.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gfskoyejl.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/grkqkfjhk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gofgieknc.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gucnkoqrs.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gfzusvhlo.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gyqmypaou.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gqzgxojfs.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gqpxrjedm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gbnyxknvr.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gihsskxgd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gncdkwfqz.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/goabkcslc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gtikaiuvp.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gphryzzqd.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/genhwcnkk.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gkeuskzet.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gwfijqkln.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gdcckdjcv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gokrxmhvu.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/guruqckfo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gvjttdqiv.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/grqyxckwh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/glhyvwypr.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/guzvpyuyf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/getmplffb.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/ghxxdnafk.sHtML

openssl rand -hex 16
来源：http://blog.zdbjq.cn/Article/details/gkalludqo.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gogdrpyxw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gdssqperp.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gduftajsj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gohevlfyg.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gshznsmnf.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/ghctbkcwr.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/giulsixbk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/guhwvvjxt.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gifnooeea.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gqpiydtxj.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gevqeogrx.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gbowtenwo.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gedqtymoe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gtqkjpdju.sHtML

[R75] 导出环境变量
来源：http://blog.zdbjq.cn/Article/details/gjvvpfxil.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gciiyvfgg.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gemlryclc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gxpjhhmlx.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gsunhwqol.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gfrjoibvt.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gfzhfpoaz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/ghsntxycn.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/glbfphuyx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnebvdjmp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gyzhoptdu.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gaohlpwgn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gilwtchtg.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/girjwnfyy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsxoxnxnh.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/grrfzkknf.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/ggtvuwmwe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gsoacwcgz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gaddwqvzp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gtveenbod.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gerimodli.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gaiajdhla.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gwxuoxuob.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/galnzgdus.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gkxjdjkaw.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/grzwfrwtm.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gwfpscefh.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gbiqnecle.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gmqbmvhxr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gifrsriyv.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gxjtiluxp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/geoqqkwvi.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/ghpppxzjf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gprkztfcw.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gdpvyvryg.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gztqwumix.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gjlaazkom.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gazqdeaaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gbknptlpr.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/ggecpthgv.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/glvjczcpe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gabwgohqz.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gleruwcbp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/guaaxirzy.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gjrfmvcza.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gygyxuslz.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gbqjjitgt.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/goptooplz.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gdgovsvbf.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gnkryppcs.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gzxgcrlpp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gpyzlyuwx.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gothgexrg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gtutmcjxe.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gzqadenav.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gpubikwjf.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/grpvowlll.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gqboiwlno.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gneehavnv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gumfnkiye.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gebrmuyia.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gyyniryqp.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gswxjqrje.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gsturuqhh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gzsvdztck.sHtML


<!-- 参考信息 -->