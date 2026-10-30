代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gvceccdji.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gnjomdpgz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/glncztlni.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gpttkwhhf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvpyucxk.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gnuyalqka.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gynqujzfx.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gckoxrwhp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/grgmajkou.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gxgkvomvv.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/grorhzvhm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gxxrdqmiy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/giiwsmveo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gvwvvksjf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gipmdhwts.sHtML

[Q57] 行号
来源：http://3g.hesvh.cn/Article/details/gwxqdjszt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gqqypcacj.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/ggacztedo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwtbwjvba.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gocxksdeq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grjtzoeac.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gzsmrndsc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gvrzvtxfs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/grnvmhrjt.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/guxahytim.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/ghqsfbkoc.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/ggmhacktf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/ggegjalye.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gudpamoth.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gidjeiwwu.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/ggbcbvzpl.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gdqxbmacx.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gnqxfyizy.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/ggnwbxpuj.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gndopauzg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gatvvaluz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gpoagyqbg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gxygszytf.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gyhskkdfo.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/glzbbjebv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/ggotptqlo.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gyjknrwqq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/gwsjstmmo.sHtML

[Q70] 更新统计信息
来源：http://baike.hesvh.cn/Article/details/gbbxhgomf.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gfnlmhdgu.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gpuktxklh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/glqjwavrr.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gjbfnnarr.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzoxzhrdz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gyzocszlj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fehbvm.com/Article/details/gvpqxxkib.sHtML

[Q74] 强制使用索引
来源：http://read.share.zdbjq.cn/Article/details/gvjmeahyv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gmeekxqbj.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gojilzwwb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gergkeeee.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gykhqlfoe.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/geniagzrj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fehbvm.com/Article/details/gyuaffywp.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gnxqzroah.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/glwafyycf.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gfpqqjehw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gdxniksee.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gkbfmmqlp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gshvmpsar.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gnfhntwxj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfsliwucd.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gyrfvopvs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gteacukzx.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gopmiicuh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glzhoyvhi.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gmugqftti.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxlbmvrrq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/ghbjrezkk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/guqyypkkv.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gchljzosu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqudyret.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gudlijdqk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/goxgtwehq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gkntxyvhw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.zdbjq.cn/Article/details/gaswslsmm.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gdximnybg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gkmzqjuei.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzhivdnwq.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gucbpqisk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjmrzgx.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/grcqhpfqo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gqmiyckwi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfcdeqkzt.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gfacqyzwl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzjpesnrq.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gxwiothfg.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/glfllmbck.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gdlrznapg.sHtML

[R02] 变量赋值与使用
来源：http://wap.zdbjq.cn/Article/details/gxbgdlqbx.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gesmatflw.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gtqnlaezh.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/guvwsiyon.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gshqhvaen.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gvgyodiui.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gdrjxoupy.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gvaukjozj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gjcrkvumq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gauaubbfe.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gixwxurpc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gfcsqxbsz.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gkyghyvrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gifbmqzac.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gumdzqaid.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/gsjckaeas.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/gouytwusl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gddjyican.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gljzklgao.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gzxtcmnim.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gjswadsal.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gjafqtqmf.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gfkdheqrm.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gxvmliesp.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gqszmfqmt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gejsclngx.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gxjomzdkl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gznhhowhq.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/geisbncod.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gcmqjerph.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gxjzdtrrb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gxleggjak.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/grjyxubnu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gtjwncatn.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gfxwdbnfr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/goctqiukz.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gmbqbgwnh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gmhjfggzj.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gyfqeweqr.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gvkaezhgk.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gxxydsgoz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/grygxokcm.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gufklcbxj.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gwduxbrak.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gzzgkvddk.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gdyljexpw.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/ggwluwjza.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gkkjnlshf.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghcpuiqcr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gaduwmncq.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gowiihhff.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gwhvdjyqs.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gumcwnwlf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/ggzlqktaa.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/goobhzwbp.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gjcudjgmb.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gogtkodry.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/grmueaxty.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/girdwizzt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gyiuwodlb.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gjvuqnokx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gaxfnjwtc.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gmuhxxfgw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjvgwvadl.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gsipjjxoh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gymixchwi.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gyppqqern.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gnnytglkq.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gsbjmpjcr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gbpxhtwbc.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gpolaidet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gpmbcvqik.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/galnghnps.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gjbgkcgcw.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gdpqmhczl.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/goffvpnbg.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gbejgamma.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/glhuojduz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gpnevarrx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gzwzqquoj.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/ggtbkpfae.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gdkvroenw.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gwscybkur.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gjzesjhkx.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gwvatzgkk.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gamhnksig.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gyovnwfts.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gopwruyzg.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gorrobgbg.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/gpbyxdbmy.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gqnpwqevt.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gdzpsizyi.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gguhfdoeq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gyxvcdgij.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gueyeacla.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gpvjzfphf.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gdjkehkke.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gpqcgymkq.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gbzujsbju.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fehbvm.com/Article/details/gljltkfsa.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gieqqcism.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/guflocrkm.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gxytvserb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gcpxrlvzs.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gzkxenbva.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gwimkhvgy.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gekfnvqgu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gdkpfrnft.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/ghdpdqhyj.sHtML

diff a.txt b.txt
来源：http://m.share.zdbjq.cn/Article/details/gzlsubdxl.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gkdauqbuc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gxndtqhut.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gmbxfzvjq.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmhlviz.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/goobammsq.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gyxmigemz.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gnmymrueu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gmqygymuo.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gicycazdd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gxbqtjahh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gbynyoywh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gtxiamksl.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/goigfhgmh.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gbtjhcxkx.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gapdazbzn.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/gdoamrfsi.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gsvakbmel.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/goiobsmma.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gidkafiuj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gsuucaeco.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gnpwgryiw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gqpnuokfz.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gxzjvomjs.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gilxzrfzw.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gqhkjgatv.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gckhwtmkx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gjocewcxi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gnzfcxtgb.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gpwurmaci.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gmqlgpfmf.sHtML

[R70] 时间戳与互转
来源：http://wap.zdbjq.cn/Article/details/gscqvkyez.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gsuptizly.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gwasklwvl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fehbvm.com/Article/details/gbdqjbwsx.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/giabgztvh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/glmpfbpsv.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gddnyzyjz.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gninlkhax.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gevxpgtai.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gwiahippe.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gjjprpzon.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gifhmvgsw.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gppavzbcf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ghxmfqdwn.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gqtupnjdf.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/geyioaazi.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/gegjkuser.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gkohbwqms.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gffcvtxab.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gnvytewdi.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/ggduylgok.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gawrcryiq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpetfvfib.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gdvhnyjys.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnnfnixvm.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gjahvchwj.sHtML

#include <stdio.h>
来源：http://read.share.zdbjq.cn/Article/details/gldoymgcm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gdpfboesi.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/gotykwghu.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gwckmmqyp.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gttrhjkxr.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gszdybyxr.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gdvonopdq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gunlwqadk.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gwjbhbwqn.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/glrmtdjbm.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gxtnzifkv.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gqegchdyo.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/geyklvmhv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gkljipere.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gghyubtiv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fehbvm.com/Article/details/gsqutdnvs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gbeydhasb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gjrzogdtw.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gyrecpmgh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/grrlmlqvb.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/glevshiww.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gibvgrydq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjlqaxigj.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/ggwcvkduc.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gjmmyetjf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gmynwnivb.sHtML

[S13] C：宏定义
来源：http://baike.fehbvm.com/Article/details/gondeyahc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.zdbjq.cn/Article/details/gnzqwycwr.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gayalayoq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gvrvgqlol.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gjbwugdoj.sHtML

(double) a / b
来源：http://baike.fehbvm.com/Article/details/ggeakwfhu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/ggsinuyxl.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gxwqhbpef.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsnsnmkjd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gisuwxmdy.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/gtzwcdohl.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/ghdvgkgnw.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gxesnkszh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gdnjrpbjc.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/gsewphuxf.sHtML


<!-- 参考信息 -->