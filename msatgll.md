代发 wailian999

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gdhdocydp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gmkwyhlbn.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gwgrpicmr.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/ggmztawtb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gqtfcghgl.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gevxescxy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gmezgaucb.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gqxdxsdlk.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gqwmbcxke.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/glloruihw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwnuqap.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/ghkybbkff.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gfcajmnyf.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gzggzteuo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gjkzoihde.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/geanemkdm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fehbvm.com/Article/details/gxpggugqt.sHtML

[Q75] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gmgvwogyj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gompvltgj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gwxtuorwg.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gmnrrdwre.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gihibyrct.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gdkzyavsv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gytfyqedf.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/ggisaohjc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/geqdwtysf.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gjrljduky.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gdyfrdpwu.sHtML

[Q80] 字符串截取
来源：http://mobile.zdbjq.cn/Article/details/gtyiucwzy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gadkuongf.sHtML

[Q81] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/glxyscuxr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghwcuhjly.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gflnfhimk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnzltyqku.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gytjhywnn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gkvptlooi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gzrjkyzsv.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmyauujgo.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gungxohjr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gesbfuekz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gbubdagdc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gqsjnvdac.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gvvwunkyb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.hesvh.cn/Article/details/gtukrqfgq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gtydlbojd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/grhmnpxya.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gumelsyaf.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gdtdoawzw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gimgszckw.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gvgbbojfs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gdgzbaiqo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggftdajst.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/giihddbyw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gloxhsynl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gezvuvrrg.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gzizhxayc.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/grbfkbtja.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gxvsqfaxn.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gzzjorxzx.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gkmugsopy.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gfnsavvsi.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gsspkcsnz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gckwifbxb.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gzlwudxvx.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gedeumnze.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gullusksh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gacfiuztr.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gumompwfl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gtjxkckhl.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdvpwubjs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmktwmgpy.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gwwnxgztl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/gwzvogttv.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gtbqinfad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gwgfyvrin.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gggkwybat.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/ghrsujtvm.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/ghumzubsf.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gpvzmyame.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gntogwgsb.sHtML

esac
来源：http://wap.zdbjq.cn/Article/details/gyrgvqgjl.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gmxmmibtl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gqxbfzvpk.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gcprbimst.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gfuetwktb.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/grjawodns.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gdkhugcso.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/gnaeuggcm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/ggtzctrrk.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gfbhfuzxq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/ggyscjlto.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gjrsaxlug.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gntrxgvnn.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gopjqdand.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gjbnakcsu.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gmdksrcvc.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gyccltwnd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gcgvtvqpf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fehbvm.com/Article/details/gacrunnfj.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gdlubgmmn.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gitmmapij.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/ghnlkegat.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/ghvphzxnp.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gvdvfytxd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gdcsvubwc.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/ghydkmbzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/guplbrfzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gfdhauawp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gglwsgves.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gaxlayoto.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gyjtrpxto.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gxqilmsje.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gblmgxlze.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gdklcrgdu.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gpmyukvep.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gwxuyuett.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gqhbfoxgv.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gnjnovozw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gevgexekh.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gnsekyhma.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gkqchxidb.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gmmgkuhgw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gxpbnixwx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gaugnnrlv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gsxglmnaz.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gttriohmr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gypvjyqae.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/goskcqycb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gizglfqtx.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gkxqqwuph.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gsktsslco.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gkjrbulmh.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gzxxmmpkf.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gxevvhryl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/goekncnqf.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/giknvlrac.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/griqyepof.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/godcfcacd.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gfslozuog.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/githncbzc.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/guhxrgypv.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gpatkxjmq.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gwcearfek.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gtxmcszqi.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gqoxrvjnh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gmvrrgnep.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gvdehihfs.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gnbzkjwtb.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/ghtanlnmf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gqwmnvpyb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gqxzedbox.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/ggrmubybu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyqqaxkwq.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gtieddpai.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gcfvhwvlj.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gljeebrdk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gumczutml.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gkqfksggx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gyrvvfoci.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gfqgzatxk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/geskjpbty.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/ggqjsmjfu.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gnocoqphg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gcpgfpomy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gdrxwpmmq.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gtnfcqbbn.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gmitszoul.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gvhyedbqm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gbxkohuqw.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gvcnrukbk.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gjfawddzb.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gbwuiarjb.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/ggntdqlqv.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gygctlijl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ghfyouzzb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/glfhytiez.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gjxtjdmfy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gcjjygahh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gkxmfwhdz.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gurgclxas.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gdmthrrjs.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gjskqpesr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gcrkuzovl.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gagoqwfvn.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gtkevevpl.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gbgtpwiuj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gqulcfgvh.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gmxkagwrr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gpxsfpahf.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gwxghxbwg.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gmeaxbazg.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/ghpruvthr.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gxfdfblhu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gchqovihc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gaipgqnkr.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gkdggtbvg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gcfdmuurv.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/ghqnolrer.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gdyanprzn.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gzoivxkkb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gaevwcilu.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gvopldpax.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gsxvtrvqn.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gwmoexhok.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/ggfdabxpq.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/glimjpigi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gebogxykz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gubqhmfoa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gaaegosxf.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gcahhxkxh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gjblroiup.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gruuoxpfz.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gglzhywio.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gigrxerbs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/grjzqhlmb.sHtML

[R79] 解析命令行选项
来源：http://www.share.hesvh.cn/Article/details/ghvddyjos.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/ggxhporep.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/ghdtrmlqg.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gyrtjcedq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grqyyfoaw.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/ghurmyxrl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbnifakmt.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gllcpylwg.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gerlnbypa.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/ghxxvmcmi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gfhtjopgy.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gwvsypbpo.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gwthgpyzf.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fehbvm.com/Article/details/gznrihnfi.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gqioltddf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/guhhqrcwe.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gswllngvx.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gdaznidti.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gdydlcuot.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gwpwezuxa.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gwnxiwbey.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fehbvm.com/Article/details/glwtjkqog.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gxwxzlnnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gdxulqhqc.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.hesvh.cn/Article/details/gwipekosk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gsasxjotv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gcxrlbgpu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gxzgscjcn.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gttfcmmfv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/geovqylpj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxqeoyznv.sHtML

fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gpdatxbof.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gkjcvkgzv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gtacnwgqg.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gqqddyypw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gtzsowcig.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gotvejurb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gbdtvckma.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gacrnmnru.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gjsccinbi.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gfmaaijyw.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gkbwwkjaq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gnwdaajpf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gwzuehzxt.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/goqehvctn.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gnwwxhejv.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gslqtliau.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/grgcxxzar.sHtML

[S20] C：二分查找
来源：http://wap.fehbvm.com/Article/details/gugpwymsx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gthhhnojd.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gqajimoxc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gxvkssxky.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gjfpzpicp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgembazl.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/ggechmmju.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/getpjvhsu.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gwhvetpyf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gszqpwtdt.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gmohxjffr.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/geecxmfyb.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ghplftmad.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/giusyjpwd.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gpunvkoqe.sHtML

const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grpyfpota.sHtML

[S28] C：静态变量
来源：http://read.share.hesvh.cn/Article/details/glporhkok.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqprjrj.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gxgwnotio.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gssumqgxf.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gcduycndp.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gzxsbzlxa.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/gosdjegup.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gbhkdvmdx.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gvfvsdgkz.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gpaeommbj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/glbcrmdcr.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/geownzqlg.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gszcjzqaz.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gwctkpmbx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gmokfpfey.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/gtsraenuu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.zdbjq.cn/Article/details/grnfagojb.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gnfodwxbt.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gtissaqhc.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gijjsjiiq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gvbkyxsdk.sHtML


<!-- 参考信息 -->