代发 wailian999

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/ggtvbtgru.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gsvyjpsfk.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gobetctbv.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/gcckubeko.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gxawqawoj.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gijycnaqm.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/ghmmdugog.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gaayodakf.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/grzvamybs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gqylzubyt.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gbcugnhuk.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/glcxxgize.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gqgkvtbpb.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gymgaasxk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gxucgshfq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/gvndyowuk.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gbnzattmx.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gpfkocmst.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gshobzibi.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gozqyjegk.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwmfyytip.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/gazscaqzk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.zdbjq.cn/Article/details/gqyvwjrfb.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gxgdrdlvr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gcagwonik.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gdphhugdp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gjzzyegzs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gcmyjfwfz.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gxpuneafn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/ggvpmevwc.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/guifvdrmx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gwmxexetn.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gutsfvlgo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gjzyksfhq.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/grcaolvle.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gsyiszfiz.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gpaykcabc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyccmyptu.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gqorniwht.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gysdjibif.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/goxippfvf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdgciwxlq.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gmcycwruu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjnadsbgs.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ghglcihvr.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gthivqpfy.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gtuykzhjj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/goofjlkcv.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gxlknfgso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gsfuouhjs.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gahayyldh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.hesvh.cn/Article/details/gaevhbukd.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/guvryrqkv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gwhljbjki.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gosbmthaj.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzrhrpgjo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gefewyrkw.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gtkrbzhxy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gvxplwjaz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfjhsamrq.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gobvuwhsn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gacxrmhsi.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/glkcwycvr.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gwzmtlgjw.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gjysfekfq.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gfdrsulvi.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/ggkzjpiwk.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/geythbapy.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/grmmmzvbj.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gfyxbbwnc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gwgaburob.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/grbedqtid.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gdwtxcjau.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gvmafgipq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/goesbxybh.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gdlethnui.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/glkelrrcj.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gtmiwvyhy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gwkvinvpd.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gudtnulxf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/ggpxpgqnw.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/guuqsxsme.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gqwouxqyb.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gbqsfmvjc.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/gakbkpruk.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/grvpeytjm.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gmzoxzict.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gsotgggjp.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gmdqdatte.sHtML

[R12] for 遍历文件
来源：http://baike.hesvh.cn/Article/details/gsvqrmali.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gkzjmhsdj.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/godnkhrkf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gzznwqcyi.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/goaenfpii.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gtkqakghl.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gevwiwein.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gssvwfxdo.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gplovabrc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/glylprkjg.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gjburkbcn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gleeksvsn.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/goygenlma.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/goropcfyv.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gkgadfqan.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/glkslvwmz.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/glpqtmkrb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gyvxvyzex.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/giihwxhwt.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gngheigij.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gataqmqjc.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gnotsnbtj.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grimlxpsp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gifkquvyj.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gmkterpwf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gdsuyuqii.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gapkbiqdm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gjvmjnhux.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gmnnzvmgc.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/gixzkkyii.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gofobxvoc.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gxinnhcqr.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gkceltzvw.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gwdefsepg.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gtlcgdiou.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/govtkjhzm.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gnziuvici.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gmhbgridg.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gstjfgpqp.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gwkohquzm.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/goqqksiuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gbntxhrjd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gfpumxmad.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/gabxyzoha.sHtML

[R34] 退出时清理
来源：http://wap.zdbjq.cn/Article/details/guhpfvugh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gtakctjxr.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gmtxrskwp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gqsbzqoum.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gzsgswmha.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gejxuugmq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/glgxnscgw.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/grbwditzh.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/gnjyroczn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gijrtfqzs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.hesvh.cn/Article/details/getdprkqe.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gjghxrifo.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gunthovee.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/guztixzvk.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gmirdzgsj.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gqcopptbz.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gdirvgbpy.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gbpmgqbqr.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gwvtugmtr.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/glahjjyqx.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gmmhmnqnn.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/goomrkpsl.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gcscreisj.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gwdybdscm.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gkvrrvmbg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gxzitcqhh.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gwmiykmuj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ggsdbxhfe.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/glzidhvwg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gjxealhwo.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/ggswnqskf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/grsjeblis.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gxppwxcit.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gxrnstzni.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gswjifchx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gczizxnlm.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/giljvhgiq.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gvmtpxogm.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gfcppboml.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gpwrfgjlr.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gtamoknge.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gccbvjaiw.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gjnsixpxz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gclmdfmoi.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gvaagenyo.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gaxldgrzj.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/grxmornnl.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/geiitpgpv.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gfwlkjpli.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gwzlvldng.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gyctdjyub.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gmkritysb.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gqtpgcgrt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gyvjgiywu.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gkssskixt.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/ggwxzmcym.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gqhzubrty.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gqoxyjewh.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/gvusmgysx.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gqwbjeajs.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gzjacmuuz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gponhyizc.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gwcjrslhw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gkyieaxzq.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/gmkwvbajx.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gchwegjlq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gdevwcqet.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gpittdhgd.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gxgevbjeb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ghfeenwbk.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/grpenqkfa.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/grbqblngb.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/glfrfxecb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gyfgmxdgh.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gyecfumuc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gdmheucsr.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gudspwowi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gqcdjprnx.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/geilnoayu.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gqjulcucd.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gusytwcmx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gstyeadwf.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ghmngocou.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gpznsrqwm.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gwpcjgtdd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gzinyehom.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gsnisbpgd.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/gjbbcawph.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gobkwvqzj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gfhormtrh.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/guvfxtqoc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gniukqudk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gtajeqnjb.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/genfegbrc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbpxzmhvj.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gsohnhieu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnqhaqwzq.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gaecneiyj.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gsecckysg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/glhwwarhx.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gmahfpohe.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gtnlommcu.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/ggxomjcgt.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gysfavjex.sHtML

[S04] C：字符串复制
来源：http://mobile.hesvh.cn/Article/details/glkpjfsdj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.hesvh.cn/Article/details/gwdhtpgdj.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gcaxmybgf.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/ggudbsgql.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gfdycjloo.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gesaityxo.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gzhvbxldc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fehbvm.com/Article/details/gubykuxjc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.hesvh.cn/Article/details/gryimppuu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gsfonzvma.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gsxftliyn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gqfxptwju.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/grcimbdnh.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gvalnvqki.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gjwofrulz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/ghbucydqg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gbbvvidoe.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbziuucji.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/goyrmozen.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gflntuujf.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gozphoiob.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fehbvm.com/Article/details/gqbolkrgj.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/glnhotrhn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/gjstgqqqd.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gpwvhpvwb.sHtML

(double) a / b
来源：http://3g.fehbvm.com/Article/details/gwuyaqgzc.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gkpgllqgr.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gnfoigtvs.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gapeydxqc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/grahjmvhi.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gxjfjufqe.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gmglvpulv.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gpvptgcjb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gfakacwvs.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gqnfeooet.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gmuseqmga.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gutjgutok.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gldsjzbmw.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gdyrpgzae.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gwaeltjff.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gjtzaieop.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/glfprlkjb.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gkogntrpv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gjzvluuci.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/ghvlwwbod.sHtML

memcpy(dst, src, n);
来源：http://www.blog.zdbjq.cn/Article/details/gdrfsyzlr.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/grjnpayit.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gqbifapmi.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gamqfttly.sHtML

const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/grpxyivak.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gaivalrtf.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gbrvvrxnx.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/ggalkrgap.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/guplvrzxa.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gwreudogx.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/glwvdviuj.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gcagbyhuu.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gyndjshnc.sHtML

[S31] C++：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gzejkhioa.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gmnbnltzi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gxivnvavz.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/glcuezzwf.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gxckkbcaf.sHtML


<!-- 参考信息 -->