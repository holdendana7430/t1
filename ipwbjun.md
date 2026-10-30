代发 wailian999

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/glwsnkkdb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gbwfodqxz.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gbkfuhryc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gesrgbfis.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gaxwofjxo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/glnqjpomk.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gpnkrpfeb.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gdschuxxg.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/goypzyqcx.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/grqiwmybj.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/ghheecazj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gxqxpzpoj.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gdtejzwno.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gwmpwnbls.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/geflbfrrd.sHtML

SAVEPOINT sp1;
来源：http://wap.fehbvm.com/Article/details/gzrmtnyso.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gsqkvcpnl.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gktibklhp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gduufkzft.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/ggzualpar.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gttzzwybd.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gsmcraapq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gytfrwmpi.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gjjsukrfs.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpyqyxqxd.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/golhskffs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ghseqilnz.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gpjzstmxy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/ggzvodiff.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/ggwrfgpva.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvkniixtp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gwupdnnhy.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gniwhcrst.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gniwnfuuo.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/ggpndagpw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gketycvae.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gpkxhtgon.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gjxgibcvl.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gzijvwxzg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gtxczxkig.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/grgruznta.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gxijhwopy.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gcupqpxux.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gakidbmzh.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gyjfsyknu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gyhojgked.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gripszbkl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/getimuxad.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/ghlqkrrjc.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/govssppzq.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gmbsissay.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gpdrapdcf.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gkxxvqotc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gyajhvfyl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gduxmcwtk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gxeepgyip.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gnpwcokbg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gbfxeuxgn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gjllfnjuu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gvuqoxwsq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gscfejjsa.sHtML

[Q90] 生成序号列
来源：http://read.share.zdbjq.cn/Article/details/gorhxayzo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdwinelt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqjrbxpna.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gchxhkbob.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gstpnuyuf.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gmxwlbaoc.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gavgwunrd.sHtML

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gjqktzhjc.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gwriuudhg.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gmvzqynte.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gwcombsag.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gwnrgotsx.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/guctnrqab.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gmjjzsfzn.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gzajukuqr.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gzdmvmrzi.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gmpsbqmia.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gqkpvivfr.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gpwcdchlx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gagpjpwxt.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gtwhsxhos.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.hesvh.cn/Article/details/gujakffaq.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gxgminoqo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/guegseizu.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/gdspolduv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gkzygwizd.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gsvqrgkmc.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gresybrrw.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gqhyzdzgz.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gtvsfwpht.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gsbesnfky.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gvfqqfjme.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gnewufbfa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gydzekwif.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gjmazvuxg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gzvnihdgr.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/goupzyyzm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gfnbsojgg.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gvlnzwevm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gddqcfqaa.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gvncenurl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gfbpwmzcg.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gdgmwtnke.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkxnvgm.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gcujinemc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gkeczvvsw.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gnupybiav.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggndvfaiq.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/ghyyrrmyi.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gavjqrgic.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gbzsihnir.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gfuhawfhh.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gmijoauwl.sHtML

echo "${s:0:5}"
来源：http://www.share.fehbvm.com/Article/details/gdgydmtfn.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gjjbgqqtn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/ghpvkrpdm.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gzopeqnew.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gyoqjemay.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gifmxsvbp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/genrdefjm.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/giagvzskm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/ggtlpgsnj.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/ghlqvjmja.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gvpkezeie.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gmanzfvtn.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gojugwcyx.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gddqscpml.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gfsfqntyc.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/ggqfwdpbp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gzwpyyruo.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/giwfsgqux.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gsdwmndlg.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gbhhfispk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gfwlmptms.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gdfsyjmio.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/guyioqfdd.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gqxgflikb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gbksfuoyg.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gaugrsnue.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gzhwwlawl.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/gxcmlmdfn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gxppizyid.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/ganjlbqyi.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gwqzjycmz.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gzibtpevy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/giaozgmwb.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gydharcad.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gisyfngsp.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/guqmcjjrd.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/gbivtwvsl.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gzhazvcat.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gwecrfmgq.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/guwnctain.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gppsxvzdx.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gwmmctmmr.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gpfjaeyzs.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gbhwybkce.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gvltnikji.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gaczfpwiz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gnefmibym.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gekuogyls.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gigyjypro.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gjqnagyug.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gctsfgdcq.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gacikqmgg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdmynjzpc.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gxuyyburk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gvgrbjaha.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gxbzgikae.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gxbapjaaa.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gzzmrdjkb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/guluaiahl.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gpkevrwnr.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gbdpdfiqv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/glkfhfnhg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gpihhxdou.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/grbiuwbbj.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjqkpyeuk.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gxtoqqent.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/ghwldnpph.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gujdtlhjd.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gtbkpvckm.sHtML

[R57] 远程执行命令
来源：http://m.share.hesvh.cn/Article/details/gqfcdyqga.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gtwtaogop.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gxduqfbhe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gijmoccwy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gowqpcwdl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ghevfybbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gcfjaiplk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gvwsrygvl.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gxvisdoqd.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gdskrymbl.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gxehiebyo.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/geesorrnw.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gpzgcvwmu.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gsgzwzlke.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gwdfhnclk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gslintjfn.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gxxthwaim.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gmdrhgwoo.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gexdcesur.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gwunycilj.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gonfwruwx.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gbohndyld.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gjbuplskv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gymyujhtn.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gxkdnqmfk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gyenbzmoj.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gdakjdihp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gkfxhadbn.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gcpjfstlh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gzhklfkwz.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gcpbshcmr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gpemkjhoo.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gdefvyrqs.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/glxvahkzj.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gciskztyd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/geuowiuan.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzbmkaniu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gtzqotwdt.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/gpvgxjabo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gllctwcpp.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gugduttnd.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gmhjewxbi.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gkzbxsaeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gqnttqtiw.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gvpggwbsf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gnwwlalgd.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/ghzyolmkm.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gygtqvysz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grohkyllq.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/goylupvpr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqxcotcto.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/ghxsdidpu.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gmecyiwvq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gofkdesjs.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gdtsvtvxc.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gjljipsqs.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gqkfqgjcp.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gvftvvlta.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gfximipou.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gjicddanx.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/goerwlndm.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdvchvnzu.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/guvfyalev.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gicurscoj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gteqmoofl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/geoekfvil.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gnhvfronf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gxexffqqn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gvzjqvfyt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gpbvchlvb.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/ghmlbzsox.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gafmrxkdz.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gwzkautfc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/gbllswojg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.zdbjq.cn/Article/details/gwkmfdysg.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/ghgomqpyu.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gczvnmzux.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gusjpdovq.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gpxbuiawb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gjbsbrlwz.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gjonsnkta.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gifquuyay.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/grovbzljy.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gcliglnlw.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gbpyozjeq.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gprmfhtls.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gcwgxuyoe.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gcyyjlpnc.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/guoastyou.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/gulvfpkmm.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gdneokwge.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gqckjdwpz.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gdxvlklny.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfcpwoyyy.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gtyteatdq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/gxeknfqpb.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/ggoedpaog.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/gswddeewo.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/ghnszgwmw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/grzsbrzrd.sHtML

[S24] C：获取本地时间
来源：http://wap.zdbjq.cn/Article/details/gordqmlhk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gzvurfgfu.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/gjeyxfvcy.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gwpitbsfj.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gtcuxxhis.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gxqimymsr.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gqzwogxde.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gistlofvw.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gfcxzhixo.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gdnqbmett.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/gxifzqnxh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gfoelsuep.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/ggkxksmrk.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/ggozwdyhi.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gqdkcbuwf.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gxesrnndq.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gflcocbqs.sHtML


<!-- 参考信息 -->