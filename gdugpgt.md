代发 wailian999

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/glvkyrjoq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/glusdcvcz.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/ghfqxxmkn.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gavxgxakx.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnzlhcgq.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcneuzrto.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxpixrxn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnudxopjg.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gdsaeqzpj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fanxiaobao.xyz/Article/details/grydtfyhc.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gjsordpcn.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gerzhojyi.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/geofcrocq.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqgucpao.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/glrfpkkhz.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gcrslexvt.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gktpihmqz.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/ggesqqgwd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gcitjdskz.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/gwuxamkiq.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gojtrwrmd.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gokgnptgu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gadwnutqx.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/glcnpsvtr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/ggomyeagq.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gldrstufe.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnoaikffg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdupggjoa.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefhcjuf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gttaljmpa.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gblfpdrcu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gvhkmsmhq.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwwykldw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkxezdzk.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gknoyyxby.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvzbdrbe.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrzqiujl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/govwkkwhv.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gduugvseg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcagtngul.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgqoakdd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxnrzzpp.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxtiesxb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyfhpwlc.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gvqwyjnnl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrdpxlzj.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gzeoujtik.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fanxiaobao.xyz/Article/details/gyoefjswm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gwthawxrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhiqbbnk.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/grgoqntcr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbjeyock.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrslhgpk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gznztfpjb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbigdyym.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/glvdnerzk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gjpalrdsy.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gllnpqitf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutoxehva.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjfwfmup.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvnourqik.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gopchbiuj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gbdwdabws.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gnnffryin.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gnunfeudi.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgraxsie.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gxcqoxhoz.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkwfttjl.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjpxojhs.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpqkviov.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gzaonkhcd.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxtfmgcu.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjucbiom.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgbolxwe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsljoqvrn.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpymogtkd.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexnrryrk.sHtML

[R08] 数值比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnapbsyc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gksboycmj.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gaslumnct.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbysnyrtg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhxhfgaj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghbxtnndz.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/gpybyaomc.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhquvpjx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggghamjwh.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbquovmxi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/glailatsr.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjyyuhvf.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfllnqhyn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gehafluco.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gvxdmboku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvahwjru.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gbgsiopjt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfbnoaeh.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcwykeyh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/ggzjaursv.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnlpxxcop.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqilwhgsw.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwtommbi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaxachwk.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdjttrzy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gohvktkxc.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gloinvurw.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvxvxsspn.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbcnggti.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/geezkifqh.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmceedvcq.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyweeequk.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/grivxknvj.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtzmlltbo.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzpfzueg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/grclrbahp.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvthpogyr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwheocbfn.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvowyelz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/geeedcbgc.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdladtum.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gmxeqamrq.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntzjfkio.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gngbwlrkh.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gtjpovfdp.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gdznxfykm.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gheusshfo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gfedpphqu.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbcovqjbq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpitlwrk.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gaqswthfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbcemyuv.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywlymxvn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxhugcbt.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gamzlewuf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gdfnkdmgp.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gfczolrxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gzgfkewwe.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gjztkrgra.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/guqutmaji.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdevelcz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gkjdlioye.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhwwqdss.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/ggcqzrtsb.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbjhmzg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gxzrzmibt.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjejagew.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gkwgtfhxw.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzyvzwla.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gwigihsck.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gnbxzlori.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsojhies.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gzlfwiclu.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrbxvaci.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxcqpvqca.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvfokpct.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gdsqsogsv.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/ghohduefp.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmafflqer.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gzaipwmrp.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gkmprplzv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gilusvyro.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiorrxjo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gydhelrbk.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/gctfqyqgv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gfctrnedu.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqxalek.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gwgbhhlyd.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqinvzdk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxuyvios.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gsrkrvhgk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gfclocoar.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gutznmlwc.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwtvoizw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjoqyqlm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfxmnrwj.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekalrgeh.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwomokygi.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gfstgzfnj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfkrmme.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gziomppqn.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/ghydldmve.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnojbuln.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/grglrilxg.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkftxcfmw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gunwoywos.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfxzgbkt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogpymlnf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/glcgouwds.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/guidfxvsc.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvuomnoh.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwwwwtgv.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnhsamlgu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlvlscii.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvouwpjif.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gufaqpgxm.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gkpisnbrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gmytvzvhg.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhvblerz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gammzcsbr.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrvydlwr.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gqbnaisqg.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gcavyxujf.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxahewgv.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gumdwtjmb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwffnsrd.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gbkazxzbd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gypsmwlxb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gphvrgyqu.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqhnknll.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafpovgbe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/govowgzwv.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gadwoygke.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwrpsjq.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgtpwdw.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/garamkzzk.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gcjirykpv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gojywebbn.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gugfldlgv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzvipfgj.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqkcqogcy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gykvixixk.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/grzhrzqxb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmdolxf.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryrtshwm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyolzgegz.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gtrepjhyw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqxounfn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gqkrakpdz.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwfsegqt.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyhbsyhm.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxbwuwds.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkiudaxv.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyjzxkic.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gjyjxylfr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtgdrspru.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grpwpmfjp.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcudavem.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gocvwdfhi.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gditnizaf.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gklokmiru.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclsrlgve.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcarnvotr.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrfcmlny.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqojcqfeh.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/ggidpqokm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/grnwiwuru.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkqalfut.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ghrotgflu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhlatdsm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrlupckx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gszfjzcnd.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnvhnozt.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gipbycrcj.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gihadbpbb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlphxweu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwelvjfdx.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gqklmnlfh.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/garvcvwpx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gycezitid.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/ggmydzojr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/grhmjledt.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gijwwhfzk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gshbsqaxc.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gggzyjolw.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisgxtfse.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjjphghn.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxycoprmn.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvrjdxxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgzjkqrz.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/glvjllubr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyznxtcmn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjtgdfwu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghveopsda.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzzzvwlv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucnlnuvh.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gjvnjpjat.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqqzlacm.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gkdgiqkld.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsumuqcm.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdujcqej.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbcbxmyn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhjrzzir.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gcuyfvlnb.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/glsveygil.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gniwwzyyk.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqzpihko.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gupxletnv.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/gqxhsvapu.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdhzlxsmg.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/getpofkcl.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gcdlzrbgl.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gktjwgmxv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtecwtcik.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gwxordcjn.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/graaxfrcx.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gickfkcpv.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/giobeetws.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gihcabzcd.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gdwcbbmjj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glcxxjgng.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gadvaumvt.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gquxcgvcf.sHtML


<!-- 参考信息 -->