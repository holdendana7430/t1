代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gddksfuuh.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gzoivzogn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gtaifkhvk.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gzuqbnjre.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gvvflftko.sHtML

[Q52] 删除指定行
来源：http://read.share.hesvh.cn/Article/details/ggpecidjr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gyufyffle.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/guaprdfbz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gsjjhlada.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gavxorhif.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/goscmibxv.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/greqtkpcj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gzdetxscb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gbkaampjr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gsfiqrrex.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/goxxpkgcm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gpjfokddz.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gtyrbniag.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gxmfntuqt.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gezwptwws.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghwyemnqr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gqldjhxot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gwlmulpks.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gscsvdyss.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/ghdcnezpf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gvpqpywuc.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gihsgbofd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmzkdrmhw.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gvglbybog.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gfxsbfgll.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gcmejfaxu.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gepkdyzqh.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gcujwyqtd.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gggsznyff.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/ghbsjhsvj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gutskkseo.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gubvvcooq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/ggwwpnloe.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gdothmjlb.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/guvlycaiu.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/godsebxjj.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gqvhdqznp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/ggnqfyqaq.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gquxzdpgf.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gjxsadurw.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gipieseek.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gpagofpoh.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gaknrmaqj.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gccmhqzce.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gjiekjzrk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/ghpglarrg.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gpxepdycl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gboirchcm.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gswneekkw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gbkmkqgcx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gqztrjxrb.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gkmjsrawy.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/ghyqojafq.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gndicldee.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gjykzwlhd.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/govsmpgvn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gbbtytgig.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gwsxhmudy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gglksflth.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/goarxiyhc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gjcsnlqxe.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gdhquhunb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/gfamgcebv.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/giyapkpcy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gjwfwfjmg.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwtszoolm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gynimejot.sHtML

[Q84] 去除首尾空格
来源：http://wap.zdbjq.cn/Article/details/gbgtcwlnc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gopixdllk.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gidrpocjc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gpeqvrlpa.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gywpiuito.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gfhzqelqo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gxtnanvnq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/ghudxuymy.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gjatltkwo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gwgidcubf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdwutmgaj.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gdivqckie.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/ggyapktgv.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gbwizcdht.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/girpyfyey.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggjzxcfvh.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gkervlcok.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmzcwbgwz.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/grvkifcgx.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gcjpdginu.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/glgcneona.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gybbalshl.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gdeygfmpv.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gaobqcivv.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gylzsduqn.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/ggjamcsmn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/grynfyqft.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/gqupqxkcu.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/glqniqwix.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gtxojskvm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gszbgvbyf.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gslgvmsam.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/guetimihy.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gajwsrlxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/guommftrj.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gjakuipgp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gosmffpiw.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gksgoruna.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gcnfwhnrh.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gifoulvvd.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/grlpmcgqx.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gawawbbvg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gudxuemze.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gyobccqis.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/ghkrrplmj.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gzgkkvzuj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gbmvbrjld.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gqykvakgv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gbxalaivz.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gzjwcetyb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gzpktezie.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvfmzvzop.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gippkjtyb.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gurqjppdw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gxxdptyzc.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/grsassnrw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/glxmzwtcu.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gexuimcfc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gghlfuqaz.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gfiqzcrky.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gjucgffar.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gcsszjjrt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gsfmdkjnh.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gvvxqmsud.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gwtfxypff.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gascxkpdz.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gtseljiql.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gaybtntak.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gzsdnkaqx.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gfdfpgalp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/ghivmxrit.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gwlihgpow.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/gqmtgdynl.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzvfjskfy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/giksfehvz.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gwguwgtmv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gukrbvltx.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gxtajxwaf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gwnemlbuo.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gwjfjcaco.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/glcffnflm.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gbbmkdgwy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gcgniivnb.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gachmuopp.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gbonobwpd.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gepdzxwqk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/guwtfbuka.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gqqqnrkjm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gcykmlceu.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gqayejdcj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gvzljyzci.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gyvlowgbu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gkkbigchp.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/glkivtent.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gtmdhyfxp.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gequlrtkn.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gsnhvuvph.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gqkpqgxep.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.zdbjq.cn/Article/details/gmferqqii.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gumfypqgm.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/geotuosoe.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gncobjvya.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gbzqtdfzu.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gpfqquqdd.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gflkdcqrd.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gbwtzdhjs.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gpooeofuy.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdseheyaq.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gtsmjuchk.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/geqmhkujl.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gertonbbd.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/guyuzmdka.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gfcqyrkok.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gazcynrhc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gihwgdbyb.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gatwhziho.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gzadsufda.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gqcspemgx.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmnkwxlzq.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gpcuynboo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gmyytusga.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gsshenbjc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwkwbtpvg.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gnvmmqseq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gjobbhghv.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gkgcloenw.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/goirmtdhc.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gdqnbokop.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gywmiorlp.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gojlvmqpq.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gxsxhhabz.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/ghbcpylkj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/grqdjtkse.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gwvicjhpm.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gtrqxnvqo.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gsxqzynfa.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gqqfdkjtu.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/ggzegoafh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gfiawsnwb.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gduloyvux.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/goqmrvvod.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gwxhuqqoe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gunyslong.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gklttaiiu.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gbxmnfqph.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gqyaakuot.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gammyvutk.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/ghuhuivoh.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gjvbeudwl.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/giccnyvgn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gxmlyurvj.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gwrebuozs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gtjethope.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/ghmctzrol.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gvuxjhuww.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gtlwhkrdh.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/ggstfwurp.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gcezgapry.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/geyhcgelj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gdhwybmzq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/ghiuhxiao.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gbrtclpyd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/ghvjnhudc.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gneomyyjr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/ggyeznwwn.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/ghaiusuru.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gxjhkgsso.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gjmiofumd.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/grdtuyprx.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gxggdljsm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/glddsxygf.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gqianzuhc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gdtxzjfys.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/glsysbzvg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gzaiyipya.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gnictqfyz.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gflwfvast.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gihommjph.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/guxedjexo.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gkvzonrxc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/gjlzrqaym.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gpfijrxvy.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gjpluaesj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gclvyayfq.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gspnagcnp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkohbxady.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gczhxpgbq.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/glljcilow.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gsxadkeze.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/ggzsifycs.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gpgtgnyvn.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gnvfijxav.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gvxrznpge.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gdrhqazfq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gyyrrasuy.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/guvyqozra.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gmslwwaay.sHtML

[S06] C：字符串比较
来源：http://mobile.hesvh.cn/Article/details/gxvjezwwd.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/gwhluohoz.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gnhocfikb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gvyfipqee.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gjvqbwbrj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/glujuqlxb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/gxjoknadd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gfjzoiksy.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/glyixdrgn.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gdflcbomh.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gjzdjjasa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gboukylwc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/guxdyqtiu.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/grjsxjpto.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gxcacelhd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gmaygrzsn.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/gjqaisrav.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/grpjsvche.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gupftqfos.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gnksnhbtl.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/ghtevvsgi.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/giphmsznk.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/ggberuqeh.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gyiiopaqb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gbdhkywyw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gdqagsmlr.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gjyscalwp.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gdnyhspki.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/grskhwcyp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gnhsimkfe.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gvpoxasdw.sHtML


<!-- 参考信息 -->