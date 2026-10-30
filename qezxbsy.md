代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwbaqicv.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaxrfpps.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmlyqami.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gjtpkjbds.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxttydcfk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrqpjjar.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnzfxmzl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/goqhtjwmi.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjqpiije.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmguactzw.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gncpaycic.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqndxhjm.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnmfrqqe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvqtqero.sHtML

[Q64] 提交事务
来源：http://blog.fanxiaobao.xyz/Article/details/gvufjuwiz.sHtML

COMMIT;
来源：http://blog.fanxiaobao.xyz/Article/details/gftbheckk.sHtML

[Q65] 回滚事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gfixlgwjp.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrjuzlez.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksxyyeuo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gqvxfyldx.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gngrxyawb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxxoyxft.sHtML

[Q68] 保存点
来源：http://wap.fanxiaobao.xyz/Article/details/gckwplvow.sHtML

SAVEPOINT sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gyaoorlyz.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gycnuikzq.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhtdsggs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxvbuvpq.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/guterwcsi.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gueessmft.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvmudkpb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gswgytnww.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqajbiqxq.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gdmgwqxuj.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrqyqvif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gfhzkmbko.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgzvtaij.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/geechmcpo.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxvqfmcz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjtnhwm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/glydxicyc.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gqjwruzrt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/grkvskyrg.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdfipiwb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gftgtfisp.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gzshvbpif.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/ggxatxsec.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gsemrknfb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjakaxcv.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gzfqjiluj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggojfcmka.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmmjymnw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkiiazrv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gyutzvxse.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkhqhtag.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/guskhyhoc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbtclrdu.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gfudbdiks.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfckwxtcb.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/ghnmgqrke.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdnfdxq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gtwnxjkyz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gcmqptuin.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqegghafc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmecliou.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjwkunwu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpvejbdb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtfuakpy.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gqeuxtdaq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqkakftl.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gqnxmkysr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczjnulto.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gunbhnybp.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gtebyxkxw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiifpuvz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzegqjbfe.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnvbkakp.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gzgiocbun.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gyddvikvg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gagklvaqf.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gohpnutrj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gspzchtwt.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gssmbusnd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwtcqipz.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gqgizrncc.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvlrudgbj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdwdybjd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujboqxgo.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfblorbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gotllogyd.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfktlhf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyaihnlb.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrtabrjb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghboadfoh.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwbwvnssq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gngatvala.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixfuveba.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvnurrbj.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikqqegfq.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjumdpai.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxddvmeu.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/giaptzbzv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqflbpepj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsykwbbfk.sHtML

[R13] for 计数循环
来源：http://m.share.fanxiaobao.xyz/Article/details/giysnkijn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gankntrnx.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/genfieptm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkiqioyd.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmilybqjk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfwqxbugw.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/grtwvhfji.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlesbcgq.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gylewtpik.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcbytyene.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gakgvgrvl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvusijnzb.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gjseeoyru.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxtsqre.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/goufwfkqk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwjmlazr.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gllcdtdsi.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuggidpn.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gauxgwxzr.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxhdyoyz.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/grhgpoafy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvufronql.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaslipho.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfgflgu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwshxnjtm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjosdrfqq.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/grkebomjv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gapfjzted.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdbaclhl.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gwekravkf.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/grmwcympk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimbsofbn.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gjidrouzq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gghlwwxcx.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhawvqik.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gusmccyoh.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gdeyuxdut.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzaowavmo.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gknjrqcuo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geirjncdv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gzkltazzl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoafoqws.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gmifuzmjg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasjclszk.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gqayyoehp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gaskaubte.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhcnedms.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkzotgb.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjxpgbklo.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghpzmlxuw.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvipcntkg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/giolcstzx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpeyisbz.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gvmmgnlmz.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjtbgusqw.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gtpekrxhh.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gtgmfxiah.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnhfpiv.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffczzyll.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gltvugrap.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsnrbjsk.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzwmepkb.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gatzdyqla.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gymxvisde.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gseswnqus.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/guqlvulku.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gtuiwuzud.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqtemxup.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtijivhqo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gpklbxyir.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdsibakt.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gpcathcds.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gqsuoqyqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gtjuecpwq.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyxkhxdc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gcbfvrmut.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwzcsmdz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gxebquplo.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gmafoyoze.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmfpdxnf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gjzbwdkyl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtgqdjfk.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gficympch.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gdhibzhmb.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gptxqloqt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiqjdlch.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwtclwdw.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gknxxrqwi.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsfvbxhh.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gvoqfnatm.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvclxcsiu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxmscves.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngshnfrg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaxccayw.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/givizsiso.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gidaebnvy.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gmqxonexs.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gkaeizuki.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxajpjk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/glynlaitb.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/guwbecwoy.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gqktgnwji.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gdhxspxdk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gdojlsyhh.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpkackht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfhpjyhs.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gauxbgaoa.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gepjrnuec.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gjjodcnub.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gqudflifc.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyontxgry.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbfpsdsmg.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbwdytea.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdmlzqpy.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gfmojzynv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gmorqjqlv.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjeqznmr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmemoufdy.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gpoyldfxi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyxbttct.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjozhmufz.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswudkitr.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gxfzndtop.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gihaqfmxr.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gdrpfiadj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmxhimrr.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkamnihm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gcotpnuuc.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmlaqct.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gwbamugnm.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/guxiywryp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gktvctvbm.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmijwdmh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gngvfubee.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gicggjiwm.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gmyryequk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppzodegk.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaasbtjvl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghurwaxqt.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdahbokai.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjsimmfg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzgdexvm.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/genaryobr.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gywlrhsze.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/geymmyeft.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkiquue.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gduzjzymb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcedblsu.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmysewndy.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gomwiycbv.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gcefxecwz.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/giabfgqcb.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gsvwwgmzg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gbbqdrjwl.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gpcqzejgo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdfdglfz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtouvzsqd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gkcpwwiot.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gosixinvt.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpijumhzx.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gllercpkn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gduuwrqxs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaoarjdt.sHtML

fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gdwbaarzi.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvdcpfoh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccwjpqyi.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gibjquupo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gvkhtjhld.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gyihpqzam.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gbshsslob.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfavswwpj.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gepavhntz.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gighbgusc.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlsxxmlc.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gjkysuwtn.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqttvawz.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gaiqujmzn.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gcrnjhzlt.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkctbodu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmymeujuq.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmlpmzcdk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gtbifoynl.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgjneltt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrwiqcdz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gkohcjjfu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbbicyn.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqaqtbhx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzgzpgfx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyzeijqd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgjqdkrt.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gefajekrg.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxxqefh.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gqulapijd.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gggzrennn.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqjuyfl.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gbxqzetks.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvmxyshwf.sHtML


<!-- 参考信息 -->