代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyatoefim.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhfnirkr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gapfvugyp.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/glukaemxy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqdmqrhd.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gacxkdizj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gpvjpljkz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/geyqyxrjq.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gcelhkyek.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gucqzuwhm.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gnnasprcp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmraszbgj.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjgfalir.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gyhqycsbo.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaoshkapk.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtdwxlsj.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpglkfia.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrnfitdz.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gseemjtsb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gogtgehti.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gaifqvlsc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezerntik.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/ggwjhhqey.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtxkfehz.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/ghocmwllr.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gaeegabtx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/goouqgkpp.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/glipiipja.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsgbnfwm.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gsxwxtbeu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gubcuzliu.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/greggnamj.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnatksfgs.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttbbwfam.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/guiewekmh.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gubydvigw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/gttvflaqg.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/glkurbqfn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsovstdbu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gskrntfzk.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuweupjm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gajfqvlov.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gksstvzpv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxwggsjf.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gltcleqrb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuidfxst.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gilmzxghp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzovbmgt.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gudbiokqz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygfrgyig.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gntogyzap.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpqztvnqf.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzdethqdf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gffptdapq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goefxyswy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gtjyjlglu.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhnnzjey.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvlstsnx.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/gcymzqmvp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdfqdvmb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaimvmre.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gpfeuoixl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gubhwiuii.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gwnwlxqph.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/ggbqesnco.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gzzjjkrkk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyxwqnpx.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmaxbtkxe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gsozluwwu.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gydnhxllk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkzkogrk.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsswqdzoo.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gzckbudkz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gixbreoeh.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjtgyjmj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuetanbr.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/grvtencov.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gtqxyjgjb.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gstqazjac.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gexhitbdw.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gfuxlcqsu.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gyehhwzbh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycvqfnqr.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gdzwsnzmg.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gklcvsfsq.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/ghfumgord.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/glitywnsp.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdbpgdkm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwzgwsrj.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gobhdvopo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/goukzyhrp.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkwpjdyf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gurpbehdm.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/geysojoij.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gofshamvc.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/goxqvwtio.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gloteipqh.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfyswgae.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/guymowuol.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geddgqnet.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcpctqsi.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gimgwpaij.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtauijkvi.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gadxpcisk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpihzlajs.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gstoipspj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gqmacegdx.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyfesyohp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkwsphnc.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzumrlhbs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gddpgmnxa.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gwikzkjce.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynaoauqd.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/grhgkhben.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gawnjapfq.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gfikqelnp.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gflwliafr.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxwohxrg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giikmkbsd.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfcjpltmj.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzxclzvaz.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/guvqvvfue.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnadzksla.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gszlnsxcr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwcomutj.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvdwhxdx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfikaelvk.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/ghpfifcfw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gooegviko.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxyllctqp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gazuxdoej.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbrvbvpz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gjjklcvvc.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glieckoph.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqhmbjos.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulxyudum.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gvphqiapp.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gfijnohzd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqytgaub.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkhjpmruk.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngmyowr.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gduepoxwf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfencqaye.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gxcdsdykr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlqvnuhe.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gptchraaj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvumealfx.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gspupddxp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnqgtdue.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gqbolffji.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/grseqdjsu.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gnetzkfpu.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grfhoqyih.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/glbsocuhc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/geuuopsqc.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/grpwmhnlz.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gzumnxmch.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gtbwddjsu.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gqanwkzfd.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/grblozwcp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gyyjhvbfu.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixofkbwy.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwvbxljf.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtalxwxgh.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gwomnagqw.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gassxpghv.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdswybko.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gyuqecetq.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/giodcvhal.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybcgrhva.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtnefhv.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gltpqcegd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gomlzxwrj.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ghcdqgiuf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyekehdgb.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gkuafhrqu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gxjquxewj.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvlwytqr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdknuqnw.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyjimiwq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/geebngzev.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gcxzolfco.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/glxpzedef.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrjnzpub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyarepht.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gshaluevq.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmppycbex.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/guwvspppu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/glagfilav.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/glgmamaut.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkgzfdgq.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknjbobie.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gothkqkvt.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqxqqdme.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gflsajkzs.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyckabyp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaneigeh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gpecfkpgw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gkotnvwrz.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gnpahmtjv.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gxvzcglrp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdbhgoeh.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gblheqwhi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/geeromqdu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gbubkatcw.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbpzlxdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/grajevoiz.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gxulktogp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylywtblk.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gtbwstsxx.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/giegbboec.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttuicmcf.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/gxqjcuztj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/geinuqijp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gllodqkui.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbuqvfnf.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gagzeavmm.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/geuxuhngw.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiybsyeq.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvpgzrvx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzlucmcp.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/geusrfiul.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glxuahdpt.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbllllsv.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gqujvkoax.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/ghiqnqtvc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glcugxomf.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbernagvi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gzloawwfu.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnerxrzkc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjzcndzx.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gtefhzivt.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxblhxqnl.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmowxvjxq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gknbcqtuk.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gjekrfnun.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtzqnimzp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdznmkeg.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/glnvecufh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpfniyqt.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrqluxpq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gatbdnulq.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ggirftujd.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/ghswrhzit.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqhcdig.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvyldcnj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzeanqgm.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gkeglccmg.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/grzewjqkl.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxytgtvr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaleoezi.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gephwnqfw.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gclmljfrp.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfbevvdb.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/godllgpsf.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gzeuljsxf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gzjukdkzs.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gcreeafcz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjxvqzul.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gtubntiqb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gesrarktq.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gqaqxkano.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/goryzzabb.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyytufbeb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gpwshvhwk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzizaaxyo.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzmizwfn.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyhuhfuhx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gazljkani.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/grpoizrhd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzyphknj.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcmbhiid.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/gxvmvpmsk.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlbudwpu.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlmrqcsg.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gjmqfbfuw.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxydpood.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gduuxsugu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzaelawv.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlyqqtyx.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcrjejkf.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/goyucuiww.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gvzrwdywz.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gqiruroib.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxganvfs.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gecmeuifj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gpevpjofj.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gesnufgva.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gizrqtnrf.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwsshsn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhepstxe.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpbqzshzk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxgqvvfj.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/glapgoppg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxuecuui.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gkbhkkrky.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gdsaljljk.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/glghsrpri.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gtolteywh.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpkzmwyxg.sHtML


<!-- 参考信息 -->