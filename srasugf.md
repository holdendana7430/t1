代发 wailian999

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnsprytbi.sHtML

ROLLBACK;
来源：http://wap.fanxiaobao.xyz/Article/details/gxgcvurfz.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gcqzjwaxe.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gofgnmodz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gslwyzbae.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvbgztyy.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gzozirntc.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwdxzhm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxabesnl.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gsytiyzqr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpameplc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrpfqcdl.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkgfybus.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gqffopiau.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gzgietdgh.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gymjynaef.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/grbxephjj.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gperyetbo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprbykkbn.sHtML

[Q74] 强制使用索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gtfeadzwb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvbtfbcy.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqxdmquf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gngpbusvx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/gjysabkfu.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzibcveqp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gfxlcepmd.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/giaskguki.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfjsutso.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/grnunucuh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gpzmercjx.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gmvhudqlk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwrjluvf.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gysvsesdp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gngdhpsni.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvsnixfru.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdudztizc.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbczekqiy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtbvuaogp.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gppjfdmet.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklejleyn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghphspdhl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeskbnrx.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/geeueicja.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqoilzxms.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnxnattc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcbvyaim.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gljufanbs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/glfxdcoxc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gscxxznen.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnxfwhli.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glvjjyqmo.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gsmxeoays.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzxgbtoj.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gslwoxruj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/grmhogkow.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjmjwtem.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gxrnduqkr.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtphpvbem.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gzjvgtzjo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkxmbchv.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnnrnzsq.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gpblpdxmm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/glzenipkw.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsatqqyjr.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gzzsfveku.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjukhjcl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/ghogtvakf.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gzufzkbta.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpffsvsns.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gpqjqswko.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqlrzccgr.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkxzgzgqx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gsgyflyiz.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/guirsfiin.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gybobospv.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqvhfewi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjlchyqhv.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gquwwtamn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgkgsmrh.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gbstrkhak.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrlxdevh.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbxfbsrph.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbyfizau.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gnjufbdqa.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gljjawhfi.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghixqgagj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggqguxrff.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvjsspzs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gsuuiklhv.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gckreiflg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnujckncu.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsytqtuqh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/goaavmoek.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnviwlbsc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gvecfosuz.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtusnxxov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyqffzvna.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gnaiumxba.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gobtegxmq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gtphzywls.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpxlnylif.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjggzmyz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgvtgbew.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glyiiciig.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwypaixia.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gyepygerk.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwauzjruc.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsorcbjfs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbrqicne.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjffkmt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxyzpmls.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gpholnpqa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxxwlnza.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmncciind.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxllwqcax.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnlrsiny.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gopzwbxaz.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gfbjlrkkd.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gnwjneync.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiqgdrey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnprqsrhn.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnvrwace.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gduyouohm.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/gqawslwfs.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcotvkmli.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyedazbf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggevpsqvf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpxlfhcs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gvayuxzso.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grswnukdw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoidgbdt.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfdqfusw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmntwekzi.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdzyzhm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gmrctpont.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gvggmfoia.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjimpdgp.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gerajvqzi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvpcnucqt.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gdvwlqdeu.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmygyqnfy.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxyqjypi.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjolrrdn.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gekkkttuf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/glpwnmlrw.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gounkawfc.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfvzpvid.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gujdvwybm.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpqmrjfm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsjwkkco.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatwuhujt.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/graulqejj.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gaguxfzrk.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/grmicuawa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gdshbacsw.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsfwzems.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpxwpyzf.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfolbxjac.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/girrliikd.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gilwcejwe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsopwuxy.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gkvowitdy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gqwfsticq.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gysbslitb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gjriguaxp.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gbkluhfbv.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitbuisxz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvssdaco.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghomawero.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gejibcoqy.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonhrjakh.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gvswbrhly.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gyeflyiig.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gttgbhztq.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/ghbqomult.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsngkzbh.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gaesmqjua.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhsrxqwd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gxljrvlzg.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfbtginv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/grnnxzrox.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gvyexxsqx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gimwuapsq.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gyicnizys.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgfcpeef.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gydfvvjsb.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuyecudc.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/grbgasgaj.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/geysjinzb.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqckgnjnm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gtdztjheb.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gvzlnbapi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gofrsvdxe.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/ghsgooaai.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gmgdszhsq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gazfiqiao.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gjpfxxkxo.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gyqvhbfvv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gokrhiyeo.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gusmgomtc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaybvsvqa.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfwwlzjy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gwzxxqpiz.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gybepfzfr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gtvpibhpn.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gavbatcuv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzxigbnwm.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gvrnftyam.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzylzbxgl.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzprcsjzf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grgjwxxpl.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnaobfide.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gxcsvhcfv.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gftvllowu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gkqvebqad.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipxbmer.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfcqcozc.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gjxsirsjl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzhyrodq.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gmyirjwrk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/goevrvtmp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gineqanav.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprzuhxzz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpvfmbxai.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gphiffdha.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guamluhui.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gycijigzm.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhcptova.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyrxrlot.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gxdoemdex.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweygufbj.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkssiaoqr.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gonkncczc.sHtML

[S04] C：字符串复制
来源：http://wap.fanxiaobao.xyz/Article/details/gwsjwuzzb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjuxkbhe.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gomtyjdbf.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsrolcwl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysxnnjcx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/grargjjln.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsvfrhxcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gynrvrgbf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzbekmku.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gjuwrlwpu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykdnrtkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gpcxoegxa.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqmizjas.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqedxdcx.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfyyohyo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gnupuosij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxxzedkl.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnqxnhzyx.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggwpnwxxa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gffwqhjvp.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gplilffwd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gmfdzcrez.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gprubykvj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdajlwmh.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzwazrqz.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghblmuuuu.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gjjjgwyvg.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsaqwqgcu.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gbquhaukg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gktpfponu.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gctdonjjc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guadagghi.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gibqtoebi.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gdgsevsom.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glcayoryx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gweyrovyx.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqiceahv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyqgqifs.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gazuhbjri.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/gcpddntfl.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gaqybdiuo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrwqwdpv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/glrkfrxhz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbpuoczz.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gxazgtxtz.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/glirhqdrh.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvgrnxgt.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtszylnz.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqvasbox.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbllswmfj.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqilospgw.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpwlblpf.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/grciuwqaq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/guagjwlis.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxwvbnkp.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gufuikqxv.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gtoyxnchb.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/guspxwojz.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/giofppmqt.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmwadynt.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvakjospx.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbnxsdofz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmkroetl.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gilfshabn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ghoeelcjj.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/guwgogqhl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaklalfpb.sHtML


<!-- 参考信息 -->