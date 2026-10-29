代发 wailian999

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gyewdbmpd.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gbqdvyfqk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gdnfotxvw.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gbpdzdpkc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/gnhwamiyj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjvrgfgtq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmbjazsqp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fehbvm.com/Article/details/gvwqancqy.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gfcvppsbv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/ghxjrqdbv.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gjyfvasta.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gpbtgygnj.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/ghxmztgje.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/glhbpopky.sHtML

[Q79] 字符串拼接
来源：http://baike.hesvh.cn/Article/details/gjbzfdkxj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gsuqspjdt.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gciwfqoxd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtkuyhlyn.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gapdmeuwi.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtfmfbwlm.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/grzmebabc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/giyzwfsuj.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gzzxbiaoi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gcqauyivd.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gbgqndqmj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grlcivzgx.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/ghnacslfr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/gowsifkqb.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gpgyfleaz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gdpkxdbcg.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gltgzclff.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gjhayuasn.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gztsoqowx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/gelnzdjsv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gksljlxky.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gealmwguj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gavfrxcrm.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gfryzrkyq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gywhigldl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gflirxzqs.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gesggrlbk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxodstlmj.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/ghccmniue.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gbhcynpzu.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gjgeondru.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gotukdpzy.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/glfqxthhp.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/ggwbwbtci.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gibxtndvw.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gofithpxz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gakjiemes.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gsurcgepa.sHtML

name="${1:-default}"
来源：http://wap.fehbvm.com/Article/details/gosempuqg.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/goeziwbny.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gfzsgoata.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gyweklich.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/guqalvomz.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsdcoyf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/ghgmwmpxw.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gvswlpizm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gxxrndyiy.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/guqutngnv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/glmvhyapb.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/gyaggmjrb.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gjrgvypum.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gqzbwhmhk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/goyuafxxd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gabogvffn.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/giwzrmnhx.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gfieabjuk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gkaossbaw.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gvbgvifix.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gskmmszvt.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gyyxfgjzi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/grkoyzrwh.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gywrrjlev.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gbvnkwlku.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gmdsvtywv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gaexicnit.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gybqvwsoa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/ghseozwvc.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gesrvrztz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gzivivawe.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gsmuhjixw.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gnmkvsbqz.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gwfmekvnt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gzkkvdixh.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gndjjtpls.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/glcxycyfb.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/grvtlcsgv.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gtmckzetd.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gihrtuvru.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/guqsxlvbd.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gursxblez.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gmgfzlszi.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gtfdbfviq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gqnmdutad.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gfoeebpnv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gxleehdyn.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gvergjeyf.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gbpooncyq.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gdfgqmvhr.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gjtmtiogh.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gtvrmpjkc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gusbsnuvp.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/ghsojnzxh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gibagwios.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gwfxihxez.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gfsoyemph.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gefcuniip.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gwtnfwrfa.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gekytluoc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.zdbjq.cn/Article/details/gkvjibmdl.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gebfunoll.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/ghlwbcbqo.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gvptuipfn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gemdthrdb.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gmmsrwzoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gdufluwxf.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gznzilgpr.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/guiamqyrz.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/gviaeixon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gqzrewmpg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gafkfxocb.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gsimelgiu.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gvpcngcmi.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gmzsonqqa.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gkpeabrcf.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gjlediagn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gxrkolcyw.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gsgiatzev.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gqlvwxkrl.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/gnfpsyoiq.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gozezrgil.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gyrilhomk.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/guwkaaadw.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gsnnmnyvz.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/grdtaggxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gawnfdfwj.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gqjveqpey.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/gwiwmvrog.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gdauxpgdn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gcckmgpul.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/gavyynhiu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gglsfhlig.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gmdvvkyfv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fehbvm.com/Article/details/gxvspnxuv.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gizplcubv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gdrceynoz.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gcfofjiqd.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/ganyyappd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gaknviyzu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ggpfsasdn.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gtufqcurr.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/grwfdadpj.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/grtriziul.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gsklclrap.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gmcypqcvr.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/grxdoiykw.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gvqeuhdko.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gpdthjtyi.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/ggqtvgeih.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/guzdpoaaj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gsgjatzvq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gboqzjzwq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ggxqatdad.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gfhmilavt.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gzpssbynj.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/ggkfeghiw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/glavasvuu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gnnmbsvec.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gnkuboxai.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gepzbusvd.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gncwdzkix.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gdahxlxsb.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gqytmhtnk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gckfbgxeu.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/goseqqsey.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gitzolxac.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/glyonubtd.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gebfhfxgq.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gdwgaitsy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/glccsqpzb.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gdqxomymo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gcjjidbna.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gioenagry.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gchenahwh.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gwdcamcfr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gcfoedgxy.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gluheizvu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gsktqykvq.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gilnqyjtd.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/gqwsomyir.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/grwxkebbb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gkoehhkrn.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/ggbijftoh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.zdbjq.cn/Article/details/gpbpndodq.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gzrspmxgv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/ghjarmgkl.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gfmjsimpo.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gsfkmxige.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gyehjcpml.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gmnkfgktq.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/ghqepdcqa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gnxonzmkr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gjthawbbj.sHtML

time ./run.sh
来源：http://3g.hesvh.cn/Article/details/gjcqrmumb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmeqzhhky.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/goeiisbke.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsrhtmdek.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gsasqnlwb.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/gtygtwgzh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gfuoppziq.sHtML

[S02] C：变量与格式化输出
来源：http://3g.zdbjq.cn/Article/details/gomrgcrdu.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gfmfavyrw.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gqnqcruki.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/guyixqjbd.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gvnjcrulq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gkrilknxa.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gwnbpuvxm.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gkcmefeui.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gndvwjqcs.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gikqmzkqa.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gybuzqtka.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/glnbejwot.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gnltjqgmw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gqlcdthtr.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gavnauwaq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/ggerqncck.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gsdarqvui.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fehbvm.com/Article/details/gcalsvixi.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxzjfaozf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gyrebqjfe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/glqhuymow.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gxmhslhge.sHtML

[S12] C：写文件
来源：http://wap.hesvh.cn/Article/details/gqbkgujcs.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gthxekebb.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/ggbumywog.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gfhiustzj.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/glnaxjvre.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.zdbjq.cn/Article/details/gvughcbav.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gytcaxxyd.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/glwkywfcf.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gfzzolopz.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gglluwwce.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/givylvxtp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhxhlvwu.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gjstyjzht.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gmgzstjki.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gnlqltoaa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gdesujkoy.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gogbxhhjk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/ggxzjyzbj.sHtML

[S21] C：字符类别判断
来源：http://3g.fehbvm.com/Article/details/gxaojumps.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/geojvqiwp.sHtML

[S22] C：字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gwmjcgtbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gayeziqxi.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gglhxnbza.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gtotdxuxf.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gfiffxirl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gppuuxkvs.sHtML

[S25] C：内存拷贝
来源：http://mobile.zdbjq.cn/Article/details/girwhumuv.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gprjyuprt.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gdizuoshq.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.hesvh.cn/Article/details/gmyhruqzx.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gbhguxois.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcawcyqft.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gtirtzlko.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gumbuyjds.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gvpzyxcqk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gjyxcbwhy.sHtML

[S30] C：头文件保护
来源：http://www.blog.zdbjq.cn/Article/details/gfniylpji.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gyovookjh.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gskfvygzn.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gtcogtoro.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gfibgkyko.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gkdksbplu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/gkacpjita.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtethrvrx.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gwzqyoozx.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gnqadakjt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gjhmrmzpo.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gehjstjbk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gwgzwuokh.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gbwzaohar.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gyrmkqqyk.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gauwplfla.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmxtervtx.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gwwhatfhu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gzlncgswv.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gvugcsbtk.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/giedxvznk.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gqqfjuddr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gwychiucj.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gzhwoaavw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gwaeegtdf.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/grsfkqbdg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gcnmqdhlu.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fehbvm.com/Article/details/gdgsqsmyd.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gydqdvgbh.sHtML


<!-- 参考信息 -->