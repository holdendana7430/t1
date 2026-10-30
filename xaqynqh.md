代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/grecubzgx.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtylfsfu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjihqtgy.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gldncsnll.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsopjwfqj.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrmemgcn.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfijvryz.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gzepdbbfz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcpvxuqw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gbyixaboo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gqshrhght.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gitaxldfp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glvenbjsn.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhzzncxy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggkokpqn.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrxilfeq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmziyrrtj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gycibhgzu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkluuvkf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gllvcrjbo.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkbnzuis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ghzreltnq.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbwaridq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnnptjue.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmaiecue.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gwyuaygns.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbblzcmlh.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gbkhfxtou.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxhepbfs.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gclainayo.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmvqdccxa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpedezqhi.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gixioiila.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmseglnby.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/giefvfvew.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzrenpik.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gluvduzsq.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gwtfjonqz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gnaxqckfd.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhmxjuie.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggjligtgl.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkmwvmdn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gwbgbexaw.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gfclqesxu.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/guqlwcsko.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gprupbwtx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrifbgbe.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gpowznjqw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjitomjvj.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkokxzllc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gpmzrvygh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gbisbjjmt.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvftltbhl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/gpbibuirz.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gqjvdlbjk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaasrwyus.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gfczkfehw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdayoxgo.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gkgxthzbq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gwstpsyhi.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gpkdwlzzs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdceryxqe.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gydamwxyx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxforegrg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/gvwzsyewu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmxstbnd.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gapecftci.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfstftry.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlnkwmgm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gnnogypzk.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gelehpsok.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzountbsb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gqtombpbn.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gezifubuw.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiollbtn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guksjbwte.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gmdhdsaps.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzwtvpgk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhphzxix.sHtML

[Q89] 判断表是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gpdrehkdo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkwzotkx.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gelgurfwk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/ggbfbfjxy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmcgkhni.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gcfbdzupl.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtrchrvg.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtosyodk.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gynwdnnkv.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gyzurmkng.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkbdrnqa.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqniwgfkz.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/geanfiita.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gctlrgfll.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkeicjra.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/ghprbvkau.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxsvvytu.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/geeyscfmy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxlkgoya.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpvkbsoz.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guijxeoeh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gktywwetd.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gpkymqoce.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbpawaso.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gvienyphz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gtgguxeux.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/goyxdcjme.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqolfnpqo.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gcrtkdixb.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gbijfmoag.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvzobped.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gthgetvtj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gpcbxqwmo.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/gcitdwniq.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuhonerc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gvavlfexx.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqbywcvp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grbnqrrny.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkremanwx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gppimocbv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpklouspf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpjqicrtu.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvogbon.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhbcanwz.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gvsehesvf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gskixgnrb.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxeuxykt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqhjjmf.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/grqqkosvg.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqfsravn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdubzaghj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gykvhojcd.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/grljvawcp.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gssjlduvi.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gjwckfkaq.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gokfhiexz.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwunijwih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbaeqzol.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gaazdiozv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsdyzokq.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gtrsojfvk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvmfjylv.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzxkiszb.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gjbaizgul.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/ghrlytxmh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gtrjtfgwf.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkithhhq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gupzeivfe.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabnedzsr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gficjhypj.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gereswpvt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gokuiqiay.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwzcaqqx.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gksybgxaj.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdwubyiw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gypyhvsku.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhdqbhcw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnqqqqsv.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gyerqdwed.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gidvlytxp.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gmxpianam.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxoczmox.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwodzmvr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpoytrgt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guuzsqvwj.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gdgvimsjy.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqywbrzc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrxbsulb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawqbzked.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfxpzwnz.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuqxftwy.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbdxrds.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiiapfol.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gerprgejs.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gqauvjcjc.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsomvdch.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gnerwevtb.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqftohr.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gvjatmoeq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthaawayw.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltgpjep.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gyktkrwat.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gvczdcceg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/geenakusn.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthtkrcqs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpvgstku.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpvcuvht.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclxtqbjo.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/goezmavvf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijueith.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gruqulgjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkxjhkma.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gdawohgzg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gghnvlocg.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gbugyrlga.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gytkrkngv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gncrddraf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/glpquruzi.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkmylameh.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgngeolj.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqvtwkpn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gohkdyike.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlwtxffc.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gxphcazwe.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsqunamd.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrnvadss.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvikcbykq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfajyzlii.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjhtkbmd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/ggcsjkbni.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnenebipb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggydhchtt.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrmqckgp.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gjqqmhrqg.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggrglquja.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvvuxoma.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gigoupiks.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/glajmhsea.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyzzfwpd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gagbfqjcz.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiusgrsx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/giqlflajc.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gjcbjqzyv.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/goxbiszza.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gfrcyutcp.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gyduczgob.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gdnrccjtg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geldyvftx.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilcwtvqb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/geytwhfkg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfcovnvb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gysvthleg.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gleqhuiml.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/grbrdtaoh.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdfhttlr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gaitzoowr.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxvyjegu.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwvjfxbp.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/guvvmtwxc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gswbvtyiu.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grbysipbx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gtboiwhqo.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxcavohc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gxttpwato.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyliakga.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gmigyegzu.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gsazkjosq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gjykzsaus.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gzklnepjc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnjmwyfx.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gglshwotk.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgtsfzlp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvmtfqte.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkdozncs.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gqupyqbfb.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gxtehzaex.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugsqlufb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsldfqpz.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmqzmghce.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamfutufo.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/geomkvdpk.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyklgjun.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gmqpsudky.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwyprze.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvebdpztf.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaihcmaj.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzzyfcfvd.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqqhfdbf.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glstozyuv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goesoawwv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gntdzilaz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojljypks.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdccrwjk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxqrevcb.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzasfnqo.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/grzuhoesc.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giujqbjsg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gffanrsrp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/geyohttkd.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/grtcjioio.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvchskfl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaiwozbe.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/giptgrwjq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gwsaxcuaf.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gnvumshox.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gifneizzw.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/grzrlhptt.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gdurtmtva.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gonuiucuc.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuohibrd.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeaxcdrc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqdghhga.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/goumqxsmy.sHtML

int main(int argc, char **argv)
来源：http://baike.fanxiaobao.xyz/Article/details/ghcffodhu.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpmerkw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqsjwwte.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gadkckjml.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgreyvyj.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/glxctzhgt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/guyiaxsnn.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ginvlcxlz.sHtML


<!-- 参考信息 -->