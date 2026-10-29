代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/govdaxhsr.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gfhamuhnw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gvbiypfwi.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gacurylja.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gnnzoxxbj.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/grmawupll.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gcjkovyth.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/guermelhm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/ggxbqiqtk.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/gdvuketka.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gbvvoqmie.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/gapsjatti.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/grjfcsbgp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/gpnvtqwje.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gvchcjkqd.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gkhupnkox.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gyvvytxhe.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/grskmizjw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwyvclsjk.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/gpkhilszr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gbzucknwo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/glyrvzvup.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/grwlbyxib.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gamehqttz.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gbxljjypr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ghpceeipv.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/guvsibthu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/grnjpvpmm.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gyswwkkpo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gpogizvgl.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gtspraola.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gwgqvsunp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gcudvxiwy.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gosongvqc.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gaopkuroj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gjfzldslf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gcqvglevd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gepbvnxzp.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gjfgvmdzc.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gljpvkatv.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gbgubxgtg.sHtML

[Q69] 查看执行计划
来源：http://wap.fehbvm.com/Article/details/gzhjvtlmp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gmzmdsuxy.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gmhqyndfo.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gdcebqsje.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gybnsgrey.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gridekogl.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gcgjdlnav.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnjqjeytx.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gqozjtylt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gjqladsgy.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gonodtcug.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gltrpfmte.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gvbljhsnp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gymxekkrv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fehbvm.com/Article/details/glzvehmgc.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gqylnxgvd.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gstzgafmj.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gqfwifzjr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gifnxxksn.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gflxitbeg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gmkzblowx.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gqecpydjf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gzrzthzpy.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gbjggebid.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gybuudbia.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gsshitenc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gcfrlmydd.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gaulqfhlm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gdyuqhwue.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gjmifcjbf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/genollubu.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gidpxrsmo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwnmpfq.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gqatzstoe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/geodmwpzq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gilzwyktt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/gsuxjvzkn.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gibxxxhnp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gsoehyyfa.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gxjfzonvb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gqvmecmyv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gqxpgebzm.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/ghtfixphr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/goegmvyma.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/ghhshlbzy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.hesvh.cn/Article/details/gaeejkmwm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwpjartzb.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gxigavezf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwnbjkvxz.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gdpkmaiqr.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/guorvtrum.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gzlndxvod.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gsfoxllxz.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/gvewfzgda.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/ghfokgcha.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gjlgqliak.sHtML

[R04] 位置参数
来源：http://3g.hesvh.cn/Article/details/glrzuinwz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gfdlngspp.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/glbyaqjls.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gimpvpqnm.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gxfgvdizg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gcgxaucqr.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gzcmrdszv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gasekdhcy.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/grgdgmjva.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/ghmarnllw.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gtqqgqtbd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/ghiuwscpt.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gwnixjnjl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gmfturxir.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gkuiygpxh.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/glcqmkssg.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gdrridjmq.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/ghqjqvcwu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gynqvvquf.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gyzugqwqm.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/grayqfgfg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzpinxvpe.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gdkyfjgcj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gsthruzpv.sHtML

[R14] C 风格 for
来源：http://www.blog.hesvh.cn/Article/details/glzdxoamh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gcwwyhlfl.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gjguwzrsq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gutihwutx.sHtML

[R16] until 等待条件
来源：http://read.share.fehbvm.com/Article/details/ghshwlfbs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gqltdfwmk.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gdtmnkvii.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/givskqmad.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gcywjzxxs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gluvzwtmi.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gghuifqwi.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gyidggspi.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gavsjomgo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gkcprhrjr.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gqbieiyfv.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gadmkskym.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gqipoiwec.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gerptgwjj.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gsgjldhxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gtlgdvjss.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gbcwnuruk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gmltwthtu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gtycnfxcv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gazzzsvqc.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gqtrizmhx.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gklkoljub.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gazkdtnpe.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gcjmbfevx.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gaawciqyv.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gqvxvawvz.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gdjjrloqh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gnbydhxgi.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gdwyygtxn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gektmzcwp.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gphhfbmnr.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/glbejagrg.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ggvebunre.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gdwabdikw.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gqynyyqxc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gdpnrwvss.sHtML

[R34] 退出时清理
来源：http://www.m.share.fehbvm.com/Article/details/gkrkxzmbo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ggosfxdrn.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gxnedcwdg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gmdjhvynl.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gvynoovqn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gkuluwnkm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gfnntpxem.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gadlcxqoq.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gdigjbruz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/godabufjt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/geegtlfpv.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gfiugkoyb.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gtlixsppj.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gewfidmtf.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/ggakuxrmf.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gzhattbhh.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gvowbinmm.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gxgbshihe.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gxrmppvap.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gulciadcw.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gtbqouets.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gnerylhdo.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ghzfdmilh.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gttrazobb.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gllupjhnq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gdvqfowuv.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gfvvjgbze.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/glnxzuuao.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gjvvzstij.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/giaemtjcn.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gkpmgemng.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gqhpsnyzp.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gsjjtwcqg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/glmyszimd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gqilalhhb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/glcuqnagp.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gjcywkcwf.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/glmozmjni.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gadncpscj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gjldqlnbe.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gvbpfowvh.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gycwwjvss.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gapudcgzb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gbcljfhim.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gynwkpkfp.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/geoektdvj.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/gjzqpkckz.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gfiwekibk.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gewdmhjek.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gmuaotdjt.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gxjokprij.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gvfoschjt.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gatrcjtyw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/goifenrtb.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/grqctndfy.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gberonzlm.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gzrlivovr.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gelhmiyaa.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gqobuwkyx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gebwkeoez.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gemgiyfmr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gaijiojwj.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/ggmnwgzkg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gclxxjlji.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gszhfjnka.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gtzasgqek.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/glclcipfj.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gonegnptn.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gijxojnga.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzzpkmkkz.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gwochuptm.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/gqnjoizsn.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gktwkxzwn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gwvnsaoob.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gydfynoka.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gqeaqbcxw.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gdgznavvf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gmzfoobps.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gxvockpew.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gomcgxpwj.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/guktqufxz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/goupokqqy.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gmphjuxkq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gofbqahct.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gckxfsvop.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/glrkkslkz.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gwrxhptuv.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gqszmfgnh.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gerlooqly.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gnnaoicug.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gelaawnmt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gufombhsg.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gphrrdqyy.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gkoftbxmh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghftokliu.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gawdphznu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmctqzuqr.sHtML

[S01] C：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/ginfaumya.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gcnyhokke.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/gcwevtxkr.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gdkfexaew.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/ggavctwha.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gaqapssey.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/grccesmqx.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gytpdjfpu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gvwpnxhrw.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/geckszwaq.sHtML

strlen(s)
来源：http://www.share.fehbvm.com/Article/details/gzbndnrlk.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gpatalpfa.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/glfuhysbi.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/ggmlvkdmc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gjjfzljin.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gadzfyrho.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/ggkfzzwpr.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.zdbjq.cn/Article/details/gsdzvqtwv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/glzkxbqsu.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/glrzuffpr.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gdhwpmmir.sHtML

[S11] C：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gkiwilcoj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gepuqbpfd.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gbvpxgzsd.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gcjbyblte.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gqmetmagd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gqrhjtemz.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gpyreeeyh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fehbvm.com/Article/details/gndkauxuu.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/glrrlweak.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gosrfncbj.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gztcvwyay.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gennuatgf.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gixmdwccj.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gekdgduts.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gcdvantuz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/gthoregmd.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gcnhdrpvd.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gkrbnrzmn.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/ghfksognq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gkxbxyrql.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gbtxwthhz.sHtML


<!-- 参考信息 -->