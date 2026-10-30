代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gwelbpptg.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gjxfamqxe.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gytutygov.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gpqbdnxew.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gslrzbtyk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gahpulpdj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gblidqmpx.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gugbwqqtr.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnzlnnpw.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gguznvcag.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gkdydlupu.sHtML

[Q59] 分组内累计
来源：http://blog.hesvh.cn/Article/details/gjbzssjkx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gphjpcnjo.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gxjolgkwq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/ghtepphwb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gwooaxwvz.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gzmnihulg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gimhpttew.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/guvcsscqi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gdtrmfauc.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gmfsdgkuc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gwfxcpgkg.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gyuyybyhy.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gcpaabhmf.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gjiiofdzn.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/giomepofy.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gpbyutwll.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gfwfkbhcq.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/goixnvbsf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/glxxwcitk.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ggqgqhehn.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gllglwcdp.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/gtapyhqrx.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gjvmpmnzq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gytuajdql.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gscukojag.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gxsrpjzsl.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gcngckeyk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gtcmwjovi.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/ghjomkfal.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gssmbgvge.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gvqogbqsh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/grgiqelhd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gwrmmngpq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gvdipbhux.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gzmlhaldh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsfindnrs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gkzuyrxfn.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/glvmsdkkc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/ggnjfnyts.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gincrpiwb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/gsyxrodme.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gacadcyza.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gffwzhhlq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gmmpjeamu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gwsayohen.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gcrsqinkr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfwliijnf.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gvrqkvynh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjvkbiine.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gtdobzpfe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gutrhxxeu.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gqrigemha.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/guamydiid.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gaqonifgk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gppuuicrc.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gdioabzlo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gliimyjmf.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/glkwdbxep.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gugtejaod.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gcdjfegzh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/ghnbwziek.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gfdvfpxir.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gcnfwjecb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwmotjxfr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gbagqnvsb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gsgpqujli.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/grunazuoc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gbllniemq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gukvcflqj.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/glgunzzbq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvunkiqss.sHtML

[R01] shebang 与严格模式
来源：http://m.share.zdbjq.cn/Article/details/gykiawgfj.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gcegiglpk.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/ggvrxmeep.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gfpagnyrw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gbpukcsqf.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/ghzdgtmtg.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gymzrjeml.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gwbvoirzu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gmpnmupao.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gqernfylh.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gwfsiywce.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gtxrfabvu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjrmnblus.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gsqnbrpze.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gczyinthl.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gpujnsxnt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gnfxovnqk.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/ggmvvpzzd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gxzhqenna.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gibijfdjg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gnizaftbc.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gqtynczop.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gvyvpgbkf.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gweyxfzpz.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gjcbzyilr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/goqypqmrn.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gqwlswunr.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gjdxyscri.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gptitvaxo.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gutcahjlc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gwvechjiy.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gqisfzwvp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsqpvkebt.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/ggjdsmvgy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gdovmyihn.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/giodomkyr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggkutnsmn.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gelwskjfh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gvocisdgl.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gyuhtydit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/glkiqlrgd.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/garphddtz.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/glyjrepuv.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/glxvdayku.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gtbddusqe.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gizptgwrp.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gcqkhjvoy.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gkihhljer.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gzumulinj.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gmgurkflh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gtygvsvdl.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/glkpiruir.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gjguwqmct.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gtkgqgiby.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gjlnpnasp.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gsttwgbth.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gqdssraoy.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/grxsodblw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/geqawhqfv.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gygcaqrti.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gyopzwmld.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/grvkcnovq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/ggadkulmo.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gqngkjswe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/grcisxcwb.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gltnjcgcn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gurdtmolj.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gcjzvmyiu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gqaofikzx.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gkxvpcmhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gyavefcvs.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gchgdjenz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gcxjweapi.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gtmgzrehp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gmippafod.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gdsapwdoc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gxizoudqz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gadhyetft.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/glwpkhjsz.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gqctnsaxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/giqyjsosr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/ghbtxzjcb.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsaufolzq.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gtyfzthua.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/guoxuhxsv.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gbygmznkh.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gbztuyudv.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gicumbply.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gfclracvb.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gtubjayjd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gvngyyncm.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/ganffwwlv.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gdsgrrdli.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gwptdnrwr.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/ghgnptpxp.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gxkczgkxr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gzxzcpmrj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gjzaqdsje.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gqapzxufa.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/ghpgfvarr.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/grbkfebif.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gbjfhhwwh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gpraycwhe.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gbylbqjyo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gpgjuvkzw.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gmagbjjnw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gzwfcbyha.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gezrcoype.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqeourkhw.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gsnrzwvju.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gictqftfc.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gjbjtfern.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gayfjgrrv.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/ghxhfnuml.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gbxlkbbuz.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gnzyojrib.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gkuuhdghl.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gnfalzjts.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gozpetcgc.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gewbugolf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gquoyxilc.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gcshfnfhl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gxfvjodro.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grennhieh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/goaqawuyn.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gctbgqhxy.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gwqpecvib.sHtML

[R62] 找最占空间的文件
来源：http://3g.hesvh.cn/Article/details/ggmrjzpdu.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gobfwejxs.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gpbfwntks.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gdypgpfls.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gbzfyyfhp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gfwcmajvu.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gfmwsfypd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/giaegitnk.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gpnfvbuqe.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gzczcpyfq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/grvczvcfq.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gvorlnuvp.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/ghueyllqg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gowyivhsc.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/ggsjnrmgp.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gttxhvzok.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gqlpudvce.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gzhuumpbl.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gqblyoxke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gyklljsfe.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/ggprrytwq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ggaukkykh.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gmphwpfhl.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/goantyxdu.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/glosnvhtg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ghobvdnay.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gzpzigzbo.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/ggxqqqgea.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gfhuxcuzw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/ggwroklrk.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gmfoblskc.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/gjfjmlxwz.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gjcvhueng.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gzlcbekwt.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/glkivqpcg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gudvzwujy.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gbrphehxh.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/gwsoscftp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfasgydhi.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gnnrpclmy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gukenmfej.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gkrzazrvc.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gsfpwhkkn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gzynhobui.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/guitcnkhn.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gjleafkcm.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/glaxfcrav.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gfnpbjbea.sHtML

[S04] C：字符串复制
来源：http://www.m.share.hesvh.cn/Article/details/grdbyjovt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gxyklmewg.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gxkllvnjh.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gzvzbjrta.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gjltfkfde.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gbydnspvu.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/giosnqqxg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gveasaqjc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gyhijiypn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gcnzievag.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gdyynjlnu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gbpowgtaw.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gfasctqjh.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gpjcuwuyn.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpxpqcjte.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/goitvlqkr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/ghgjooofx.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/giisgqene.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gvxhgchuw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/goozmpcar.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gdawgmmgr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/glhtxczgc.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gogfqwyhy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.hesvh.cn/Article/details/gcpxoepkq.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gyetumdro.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gwdkdyaug.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gtymxdcai.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gmkodgocg.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gwaaubjak.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/ghdpvkjal.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gwpjstvpq.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gfgdfofzl.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gnrjanfax.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqkxzkgam.sHtML

[S20] C：二分查找
来源：http://blog.fehbvm.com/Article/details/gyevepwta.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gldsdjqps.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gzeoorthu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gmudfzesq.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/glnxsjyon.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gahkwiizc.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/ghloevzrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gpaugwysg.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gyqtjeoqo.sHtML


<!-- 参考信息 -->