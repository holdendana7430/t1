代发 wailian999

[Q65] 回滚事务
来源：http://wap.fehbvm.com/Article/details/gsvpajrfh.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/ggrljzjtq.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gylivygbl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gkyeowzph.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/grikifepo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gtwprlxzy.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gwoycbcqs.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gnadksldq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gxcslvstw.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gknivmtjn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gfwkzyqlv.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gpakggakd.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gwtakelix.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/ggvgaqcuf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gpzpeaezx.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gjjaeztdk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gwvuttpqx.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gjmladxhl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/grtckkjks.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gzoivvjcd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/guylmjfgt.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gdxiqbdqq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggetyxwtt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gqudzrxor.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gdgsavhxc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/gwssmaenr.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gnenhftfc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gaowcnqjh.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gnnpzisnt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/gqjxlabai.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gubiuyatb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gykmnjfiy.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gnumlknsf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggsjacstm.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gzdkqbbyx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxmfjbbku.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gezezmegn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gisflvfrz.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvfyrbkfa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhetuhcz.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gsuihsycu.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gflszlivi.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/goprrpexb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gjvollzlu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gnojdurrf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gztfxqfsr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gypamvwyi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gzovtrlgk.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/ghwfrbrlt.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gvasoafmr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gfsdqxpxd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gunizkxxw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gbtwpvucj.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gwhvlrkmp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gldpnpeuj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzjjapwuc.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gnzuatmon.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghafytadu.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/goqesqpgv.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gjyvqntxy.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/grtjncdge.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gexhlcalo.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/groenanhz.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gmawdrrmc.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gyqubzdmz.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxkcxakbp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gnadapcfx.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/ggsueyxuq.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gazmclfpc.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gptztdpup.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gzgemybef.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/grckkfbzp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/gsggjxgpu.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gtajxzkzi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/glqhcstcs.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gyxrlghkf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grnydoqlc.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxirtrqcd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gwukmtjgz.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gmqqohpys.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/giquedqzk.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gzuntfoip.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gdkokqhzs.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gwimxhddz.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/ghmkfbtyx.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gkqeiehic.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fehbvm.com/Article/details/gppibtfjx.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gjwwcafin.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gmvdiptvi.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gfbycecxm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gvxudcdzk.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gugntepek.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/ggioaowbc.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/grezkrljp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gqettgodr.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gfhoudjne.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gzbkwiekn.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gyqjlsbsz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gsrimgtaa.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gmoqddbbv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/glzmbwzef.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/ghzklcctn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gkyvbfeqj.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/guhblhvds.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gdhgyszoa.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gxtrfqymv.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gamqveaae.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gyjtdocgz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/gjhdcydau.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gmrpnuaai.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gmqeyfhqc.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gjrasxqxw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/goubawxnu.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gsumlygyg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/grvmevmlr.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gejlwvoot.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gdgghjaez.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gjrtmltoo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gfvlklxyn.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gbwjiwfuf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gqgxtfzfz.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gfkexrozy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gyohkgjzf.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/ghdlxkdcq.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gccvieobq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/ghiervggp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gpmdadwov.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gcentaouq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gkhaakuvg.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/geaohysvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/giwwxviqo.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gmhjhnruh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/glzkfohat.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gdxtivqtj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gtmcuaubc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gobcwbcok.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gjfjkqrfq.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gvqzvlutq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gtshhixzn.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gzxibfjab.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/grkxdxils.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gdenjwrwp.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/glcqcbcqu.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gbgcvaaym.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gqueathpf.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/galxnqpfq.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gawvhnecf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/glmasxdxy.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gncmrhjiz.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/grqoxzucy.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gvpwuoldy.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gnetbdyxo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gagnbojzj.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gidsbinew.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gkfzgrczc.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gnnsfoeqa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gdrotncjv.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gzwomtxtc.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gchopciej.sHtML

[R49] awk 带条件
来源：http://wap.zdbjq.cn/Article/details/gmbiawmyn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gplxerysy.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gzksepehd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkinysncd.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gjzofjjts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gxqkzeesv.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/ghalucqby.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gkumzwthj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/grzpdxigv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gpqdyahxw.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/guyjuvvyy.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gocxqpkea.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gofqxgwzf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gdaptzsul.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gszyuwigg.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gmbrgoosn.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/glnslovvc.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gasrdypyl.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gusjtftbr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gvcatsfcy.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gtvprczap.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gcifvmkrh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/grcflsuth.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gmzuhqdpa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gkvnufmzx.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gybswrfch.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gtsxalfpb.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/ghkqowytk.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gdozqfhzs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gxjowkpdm.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gcguytoav.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gaccriiee.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gsfciycsp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gmadkfali.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/ggtffemgy.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gmfnnvzrk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fehbvm.com/Article/details/gtvbeevov.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gecnlwipz.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/gepshsfxk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gcvjtfogg.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gahqoostf.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/ggesnxmbc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/ggfgkzphy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gjjfnuwhu.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gvriibewe.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gfpemhfaw.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gtfswkekj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gzsvakrel.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gubyrsnct.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gfvdnypzv.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gtpvyrbpt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gbjzlajge.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gpicpllop.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/gcwervano.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gemekwlew.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/ghastbooh.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gflmatseu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gdwxsphgn.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/geqwpxnnj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gyjsjezfo.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gtqptzqjo.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gmazkdqyg.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gixgtmqyu.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gpezjelto.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjmnzlpc.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gfgagnnab.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfbefxica.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gwpynnmvc.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gqmyzugtz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gaacvjnsn.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/gibpgzlli.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gxtvvcjcv.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gjhfolvmc.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gmiglfwwd.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gmabrhvtm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gakqvmcof.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/goaqidmvq.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gxtmohidl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gojggfljh.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fehbvm.com/Article/details/grtbcajpq.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gwwuxhhyu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/gnqediggl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/ghsgqbfzs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gmpshixsy.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gwyleaitn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gzmptrfkc.sHtML

[S10] C：指针与解引用
来源：http://read.share.zdbjq.cn/Article/details/gmoqdvuld.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.zdbjq.cn/Article/details/gqroowjyl.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/grqawvewl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gqvzqxvvs.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/geqpkoelu.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/glylbldmg.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/guhmcuvea.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gudprpwgd.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/glkkttxdx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gdatxmjrb.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/givgkjnyl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.zdbjq.cn/Article/details/guekoypxg.sHtML

[S15] C：类型转换
来源：http://read.share.hesvh.cn/Article/details/gpjdimwpu.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gytbdqhei.sHtML

[S16] C：位操作置位
来源：http://mobile.hesvh.cn/Article/details/gjuzakmza.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gjivlobgt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gldyfinyz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gvmysfuvg.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/grutxxkgr.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gnyqqmjpg.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gfulcvoht.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gorghfdia.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gnrlesqlw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/grqfofnww.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ghbeloctr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gsfbjlwib.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gddmsxpcx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/goktahvyt.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/grrkdpedu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fehbvm.com/Article/details/gvzcitdhn.sHtML

[S24] C：获取本地时间
来源：http://3g.hesvh.cn/Article/details/gpiyawjqa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/ggkdfvsvg.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gjsozdxkf.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gmixzfpwc.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghrziaxqa.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/grjzoxhzd.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/glqnekvcl.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gdfujtnbh.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gbccajvpy.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/grwzkfovj.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/gyzgmwxfr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/glrvcuoge.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gxtbmljbo.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gqsalybaw.sHtML

#define X_H
来源：http://read.share.zdbjq.cn/Article/details/gadnzrlyf.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gxvjlhvbd.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gejbkokxw.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/grtgxvpch.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gzotnjftf.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdekvejax.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gcyaesbys.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gwmdjyhkt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gkmzshnbj.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gprcmpuyd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/grttgrdnf.sHtML


<!-- 参考信息 -->