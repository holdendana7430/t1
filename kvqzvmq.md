代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gaapqefwj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gcmfbunus.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdgqprmg.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyvtfbmr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxqozsqv.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gmcifywgp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbnlvrw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzuhwawm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfahxqmjn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gomofoztz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtgvsguh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmitdthqh.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/geinydxyb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gidpmhhsq.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gfltszcxp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtknhnqyb.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxtadjkve.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gzdshfbzw.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gdkbltpiq.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/guloiggbr.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gehgdwhzk.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gmnasecvw.sHtML

[Q66] 行锁查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtoqlxyxm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasicxdwf.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoqipeiq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzirmvafl.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/glzkynzsk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpllpvmyg.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glzbsrflw.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzmpomum.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fanxiaobao.xyz/Article/details/gwjutxaom.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gurvqgjyl.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmxhrusmg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbhwgpon.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gdboutvyj.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkoauezv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/givfsfpmk.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gyetflyzh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzqcxtsv.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/ganngqxez.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gygkayoxl.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gyasdyiib.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuvwgeqb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gzsnuuhsu.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpszayoos.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfkoxmop.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gosgfsdpk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gxyecvmsu.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gkqjpblfv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gvslpbpvo.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gibppcflb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gtojkcofg.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlkvfgab.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnulhquzu.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiaqxiep.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grslulazq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwerccmzq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggekifzwh.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gofvzraly.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnikptjuc.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/genchwanc.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhbjxkmq.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gzwkffzpk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gvcuthgyn.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/guuqbyzrv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gflzfepnw.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuuepxtf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gnppsczuh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gsyigompl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfehyqgs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbuochvs.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gicnrmldp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gqxorsdlx.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlmrqapt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gohxkwqqs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/guhkkswmm.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gfhknbqwg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkocjyqkr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqaudqya.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewvckesb.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiygqedp.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gsculsxvw.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/guaxvesho.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpkmpzfr.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gglykcshr.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gowvpqgav.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gdbvpamjh.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcchbgyk.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gbwlbiaql.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gkbxulgdg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdgshimao.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbfajsqdb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeltkbgs.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvtpfdff.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvfwwmszy.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gbljtsyfn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcyebbnj.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gycraqyso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gmodvinjn.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gahbslwbk.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnbyaarg.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwsdnzhjq.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gubycwwpi.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnahwqwxx.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gpbvhgrsf.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeyesgtp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsolcddgl.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gdnstngln.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/geyuwyuhl.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjaebjbh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guirbgezr.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gflbrbeee.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grqpquvyp.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcahjmqmh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnueudzj.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/grzyoinrx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjmprqgeu.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnnfhcmi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkmohcach.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gfimaecpm.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwekciahh.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gnhzcsoel.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/goumoxckr.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/guykjlhbe.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gohzqqkkp.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvuzetsg.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcnnprvx.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/ghixppueq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtnrkqpjr.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyohodkqw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghpxhtnim.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/girjpxnuw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/getuhopgn.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gqleagmdb.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gvmnrhgpe.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gizchpnno.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtftjvjh.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmgqmrus.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gxqinepiz.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guamcptak.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gcjnykzzc.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gytumkrse.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyoyehbi.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmsuvdju.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqasyevf.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gocseuwcu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfddbvifb.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbzpbjlf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjqsjbkz.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gozithejo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaqeuuaw.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gekupoqor.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcljqlsqj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdbpkcmn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gfshgqlgi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gvifowsry.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/geeyymizy.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvdogsje.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/ggadagwbb.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gxeujrbnb.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gxaaoxyjf.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gyanqrmdn.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gpaisbcuc.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gaknosblo.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlmliotp.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gndbytfau.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvueznrc.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glfimblhs.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gvydfxzya.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/ggqpjgkuc.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/ghghxfmrb.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqqkfodt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmsolxyp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gyayeadrz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqurymzot.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvzpcilf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtcircgy.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gcpebetcd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gglyuclho.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkspbbnu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxetushj.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglcceqyb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glxykihkl.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaevayqo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhhruoxz.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gonuzunuu.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtagqpead.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gnxdknpxr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkluqebx.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqhyvlvb.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gdlzqnkfs.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzzamyvz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcgmitgg.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gtkorydpq.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiprnrku.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmxpaame.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/glbicmdyu.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gaptsndxv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrjdmyqn.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvzmhzvw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbppioni.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gdundrwot.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gaihtahil.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghoamtdpd.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/glnopqloe.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqhiquykz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gbociodom.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gxeawpgev.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gupjtrtmu.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuycrbfq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmdcljeq.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/glkrrpgav.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkvlcoi.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcrsaqlj.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gxwakdvtw.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gllwpwqwh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gboilkgzo.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/ghmyytruv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkvjvluhe.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/guchhviij.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gelfrrbpa.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmzrqukpt.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/goouuatip.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxjjyoaxi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbchtxgdd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkchtqmb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbchztwv.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gksrocltr.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gsocwbddv.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdndofzz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gctetkhef.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/ggdmswdtw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghosaldjc.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdierxdgl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynajhsps.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyqlzjzv.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gfsfvhwyj.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gtssoebic.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyaavgdya.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goezfddmj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeahlzlk.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gbgerclvj.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/glavywhdu.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvbizudr.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gldopdtwh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guskcbbyv.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggqyflmna.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/gvwynkqvz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesxvwhkk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gktdolcqv.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/gwtnztali.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxrmvcep.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guahqvkso.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvaqnyuu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvststwbx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgqrizqs.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehmejazb.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzpljjobk.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcufshphs.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ganibkpyk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecwzxhoq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gtidvrfpm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gmlikfgxv.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gdujkxjxq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gkfbqijoy.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gueujmcjq.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gsprhfrgc.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/geudpouwd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gdumxglpb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsffxofc.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gaztcmiaw.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmksqboc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gmueuzfwb.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlrrywrw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gqxnbjqcj.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gycprargu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gyaftcudu.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvssnvve.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gkblgcuvc.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gxiagbawl.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzrwnrgzx.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwplexjpi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvhotmuh.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeqgqkch.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigxjmwal.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwuykbcnz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ggnaocnkk.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghftnmgrq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnmujbgkf.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/glmmztkzm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlqrnrbp.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gprwoabim.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gumckving.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gijaholtz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjypqeebt.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfrqeims.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpahhgqzv.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmlqxdnd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdlwtchq.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gtjamcfmk.sHtML


<!-- 参考信息 -->