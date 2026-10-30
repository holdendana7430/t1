代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgtmhajm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gfivatdvf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/ggntdonrx.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gotzszrhl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvwdjbung.sHtML

[Q58] 累计求和
来源：http://3g.fanxiaobao.xyz/Article/details/gkcwazqer.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgeizakv.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gxblzjfoi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvpinamo.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gofyhctcm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzwbhhmq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/guwmogjru.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrlwwfz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gdwrqnujz.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gqvjxfyop.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/goeubjkgh.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqmowxkz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/ghemcwhlo.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfvdfqjs.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbduroac.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gkwcamzrb.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahqfukau.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/guceeeyby.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghphmadfv.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gixatbnyd.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmmznqip.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gkqrwmfib.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glvubvcnw.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gwcgsjirk.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gfummmmgg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggutcjjdw.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghivruzf.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gytfdlfcx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/goayiwqen.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gztenifyh.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgpanndk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ganorrzis.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxourdrr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgzjvcce.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtxesrqiu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlgnsyda.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghatprlxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqooldxg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnwzfupe.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/geovhupmp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpczdqccz.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggoocavx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gvcxurnze.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnswtapuy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gzneeryeh.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gbllfouwy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcencsnf.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/ghensnhdd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnujqpdcf.sHtML

[Q81] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgtdlciy.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjjmdwje.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gatwwdtrm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnpzhhhv.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gsddjceim.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/giurygibf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicipbuhx.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/girfkbwiw.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gznuxnvkk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbegyyzej.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gdkkxhqyv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvgkdvve.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/garblgnvp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gycrmvbhm.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ggxzvbosy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnjndpvi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszcsiypa.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gownzizob.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkimdbwu.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gdoihfmij.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gozssotxl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsisctjx.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgehmory.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpopwgycu.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbzvjkci.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gcbshceza.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gnrfloduq.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gzacpjflm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjxyeywq.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwvfdkht.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gmoxvrdyx.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glvvtuqhp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbcaumep.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gvwznnkwx.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gausgsqic.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmdoxyqmh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkickuays.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjalbyqu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gtxuqrkrn.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghvsripny.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/galcuxyfm.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbgkdvdq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqumzzht.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gakwundak.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwrgtsve.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnnbioff.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gorumrzae.sHtML

start) echo "启动" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnenqnxuo.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzczwehpj.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnuceesm.sHtML

esac
来源：http://3g.fanxiaobao.xyz/Article/details/glxxafbti.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gppziurpg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxlhilznj.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbttythp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvvehcmmz.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/grlpllbok.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gzzmgsnic.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmeexvdmm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glsirkmky.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqrxoqxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfzndtpu.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokxgibem.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gldoiihbz.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbjpgzxo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzisxfgu.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtgjqrma.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gapccrlxt.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gpintkawh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrarzyfh.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwenqqbad.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmuisrjz.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gyylzdgam.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwnbryczw.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjsbpiwd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbkzaagbh.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/guxdidjxf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblpvgksp.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gtweanrgj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/guhxstepv.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgocppul.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/garenrzhd.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gflevlczq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gclasspfk.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/godghhuus.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gnllwgdiz.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdzgxcro.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfuikxrv.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpaloixx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gdxsmoyvc.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbkwurneb.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glzkfwicm.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcpeefjn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gywrmkfju.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmitvmzd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhexamkx.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoyvfbpo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gapodwjia.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gqdpxuvgu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtexsxgqm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gdptmwcrh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gmveuriwz.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gqwnjyibd.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/guasyftio.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/ggvnrqrsr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gewkfukpg.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhyvtzzt.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwjlnwbh.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gzgbowcnd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gehprfkcq.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvwywygl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtfzbdul.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfwltxzz.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gqawmoyrp.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvpwsrab.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqstdmclz.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqpbaeh.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqhuyeew.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gullkorde.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlondgcv.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsobdhvug.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gwzzdlfpq.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkuijjoj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gotgnullh.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpixgavx.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwaocjocm.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gorrdmlew.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gqzcdipbm.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gdfwwgrls.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyvcgvnz.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgxyuwea.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gxexeiltz.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyduncecr.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwfcvzyhq.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/grmxvfufd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/goojrbbza.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqospzqis.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gicjvmexz.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gniukxaeg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvowsclnj.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gmoobnwsi.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gspbwybos.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gdlvbtlcx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goofhcqzd.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/guaozekzh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxwhefoa.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfsnoazf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpppbcpw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/givrrkccm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/geqcwkdnu.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulmdmasz.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/grnsosauc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwoljdei.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyvneaxz.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gldbteqgt.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/girohtshx.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtsqghuu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvrlbvpc.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcufyjevk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/giyiztofw.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtygmvpuq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwuyyvyk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gwjareasl.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmrivuht.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmrfvvvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/grpwnosye.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdmhdqmi.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gvlsfkpxm.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/ggipjyrau.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gdltpyhnq.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjypmpoe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gvdcagoti.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gjwpjrasn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grvmhxoui.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gozacvkzu.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqyvydhx.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gkromxxtp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grdegugcq.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdlfsbzw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gadfrcfph.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/glgjllvnm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisrdvnjs.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkyjgpxe.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ggamfifof.sHtML

[R78] 交互式菜单
来源：http://mobile.fanxiaobao.xyz/Article/details/gdihssike.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gwxjyriim.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gicdwbhcq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhlzvdqg.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoutcyxe.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjvblhqr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheycsvmu.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gibyiqngm.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/giefbdsro.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbviwgvgh.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gmwnluojp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gnnkyadev.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhvqckvm.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gksttwclt.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gsqdxkdhe.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gxfrnyhwh.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gvonefjpo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gebcxiegn.sHtML

[S05] C：字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gobznyutf.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gectpptue.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkoxwkctt.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/glweaebxp.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gpjvwdpar.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatqtluii.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gowpbkrbx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gbbmnsybj.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gpvlzfzrm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gfohvziuf.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ganzwbdbv.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gamwsobxx.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guzphaaap.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzreogywb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/glsimjtpm.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsbpvdml.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwzkwbfz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxwdugdl.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gbjlyubei.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzlonyjs.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyfxxunq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gkqltlsur.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gijovsora.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gfpqbjpiq.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gkddhhiwu.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuqtbvbd.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpaqjwuf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnplrdxt.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwztztgol.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbaspervi.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gljosbhqq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/ghlgdkouv.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghattusdy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gsegpviyu.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gyznmphzg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhwvbqmv.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgqngtl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsihupcu.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvxnbjwl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjestoou.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/geudiuxmf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdppijhz.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gczxtiejj.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtcbnah.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gvflzkmwo.sHtML


<!-- 参考信息 -->