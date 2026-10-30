代发 wailian999

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/glbmcrdsx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/ghdtimtff.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gdbklcpwd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gzsbymvek.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/goesrgiad.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gdahnnlel.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gduanadnc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fehbvm.com/Article/details/gltovodvj.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gkohtwbyq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqdppopji.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/grbbiblre.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqxfeaz.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/ghwtftagk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ghgqpixdh.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gnpadknpx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqigeviyl.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gjniprjaj.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzrhynknl.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gdnfvipcq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gruqvhjrb.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/ggffkypql.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gfvdrfjbo.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gsqcjgdis.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gvglxifvh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gzudbuggg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gdtajtfde.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghqevcnhg.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gzxsleefc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gnbmbkneg.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gzcxvvrtw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gdhgbxkgj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnnufqqcg.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gpyjiopcd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaaxozycg.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gihhmreiq.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gpogfrppq.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gyoyrutkh.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gwrdoipyk.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gaoquytnl.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gukqkbbel.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gpwcahooa.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/glagrdwwa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/ghmiqziwt.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gdokmnjxz.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gbnkzzhnp.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gjvkntsyz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/glwnmyhnd.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gzefxdqur.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gebwdmroe.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gwdzxvwnx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/gagrdlfay.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gzplyakif.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gjirwumbg.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gezqqjunh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gqhwuxrma.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gveplvufm.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/giqygdeis.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbadsrjlz.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gxzenprrm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcoblmotn.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gqgvulsyn.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gtbymbfse.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gzopvisju.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gzlywtqfh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gsrzfmdhx.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gnjrbzure.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnsjugonb.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gmdafbxfy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gafnvvkoa.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gaujjhriu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/ghrzdsoyb.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gixccubki.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/geypwdjwt.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/ggaxyqtpd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/getwohzjy.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjzigjbdd.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gqlvczipo.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gkjjrbvyp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gcmtwlkdr.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/golahzjeq.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gfaeanzjw.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gwqytthqi.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gikcspois.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/grjpvgbuq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/ghahigvlb.sHtML

[R24] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gmjhsjykg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gsjkrkoek.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gpxvepksi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gxatoxmij.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gafoeapyc.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gvifijaoj.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gbgddvaqv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gieemfmdl.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gfdosegpw.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/ggkvbcrqu.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gmwgzxfrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gnoylhezo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/grhazgwfw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/glkmgxnaq.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/goialakqi.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsphvohwn.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gkotjrkmr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gnkgtrjrs.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gxyjnatkv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gjeqgkedp.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gygpojocf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gqpamhzsh.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gbqunxsyc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gubsujuud.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/ghiwskveh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gelgfrpzk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgvxdya.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/ghntmoamx.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/goytxwfmk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/grrooiwzc.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gbblnityq.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/grbdscbpi.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gbzdybiya.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/gvkaoczim.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/ghnsfcmir.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gjsiffrji.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gutcxooir.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/ghgtseium.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/gqbvchlpy.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gsandryye.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/ghpzkowhw.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gityzfagw.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gqldtvxhf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gqbtfolsw.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/grbrodubv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gtoawkjwq.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/gmhcsxtlp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gnfsicgqp.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/givjqrhdq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gujmlbubq.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/goxvjhklx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gttgytcrm.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gzvhjfwcr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/guvxsxmih.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gzwqfqzup.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/guypfhzhk.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gonwmfobn.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/grqemayus.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/ggtlhhmkl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gntqarayw.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gmdksdcsj.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/goxwwwvcg.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/groumhwtu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/goaqcnezx.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gfpjmngtk.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gprdzcuas.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gpulmiuhk.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gnmcbuedc.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gaxqvtryq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gvpkamsqs.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gxmxdygna.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gjmjldjle.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gwthflasr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gagapituc.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gpbiyqqae.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/goaissuvn.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gefrrsrvq.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gwnnxcwlp.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gmmsqqlyb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gqppxumvw.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gzofhqjmy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gdccclsyh.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gusrdtgpo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gawrbnvdh.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gdqzggtwf.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gxtbjjfps.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/grpgsnlad.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/guizluoog.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gaelfdujr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gmslsficy.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gwvvmcxte.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gkpccniwh.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gooyfjhop.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gipjlvmtw.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/goprblrrh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gsbjmxlyp.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/grcizqsin.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gbiorgvqg.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gyejhppgg.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gxxbkclgy.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gwzzftrxw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/ggvdpwowu.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gfuhpqyjd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gfpnralex.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/grwlxuqqv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gksvynnkm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fehbvm.com/Article/details/girdinefl.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gdfvfnrpv.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/ggqiabrpe.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/ggmiojxmp.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/glzdndrtu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gqxwevniu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gqnpvfgjs.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gkzzdhesw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/getcmxrvl.sHtML

S. C / C++ 专题
来源：http://wap.fehbvm.com/Article/details/gkftiepfq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gciiugkcz.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gunjqwoyx.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/gtkytglxr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gsehhimdf.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gqfugnqec.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gpzbasxjf.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/ggpnwkhog.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gaktgxsog.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/guuxjillq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gsqfsklot.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcokaaboy.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gwqmtquop.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/gcpubtyhj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fehbvm.com/Article/details/godfzkdrl.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gfyulfyjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gowcmpnyb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gutfmqlds.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gjrijgekv.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/gobdlvukr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/glsbmewje.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/guzwzdsdk.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gxhxplgdw.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/grxgpksgr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gpdabityb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/gywbmloer.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gsloqaypk.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/glfmwsbdx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxspzqige.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gqnvtfvvh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/glhorzdzu.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/gyccxnlyo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gnsikelvc.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/geylihkyu.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gwbipszps.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gypbjvsup.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gegtxiygr.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gfzjycucd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gtyqoruzi.sHtML

[S18] C：命令行参数
来源：http://mobile.fehbvm.com/Article/details/grcdwmbrw.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gzqusoaqq.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gmelatpsf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/gxxxlpxzf.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gqrexvcip.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gclmwtluw.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gpkwnggbu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gdhgpavrf.sHtML

[S22] C：字符串转数字
来源：http://wap.hesvh.cn/Article/details/ghfkyeywc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gymqpwsfh.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/guflxullg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gxlxakgno.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gtavncnca.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/grxqcvncb.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gxohhzvqo.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gttquktbo.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gztaytwsy.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gstlgqtoa.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gypbwuepx.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqonplfuq.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gunhqzmdk.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gtwtleosr.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gemttsdfh.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gzmperwek.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gqdnywsai.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gwvedfxvk.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/grxvislix.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gmxzhbdla.sHtML

[S31] C++：Hello World
来源：http://baike.hesvh.cn/Article/details/gbnfclskn.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ghbxaoszi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gdugutllc.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gozsltacv.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gtczjfqup.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gfgivwaot.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gdfmdnhny.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gwuxkuggm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ggczhlpuv.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gtsrpzrve.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gldgdagme.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gxoyenoac.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/giogmuwcm.sHtML

[S37] C++：set
来源：http://blog.zdbjq.cn/Article/details/gcjlsyvzx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gefweoirf.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/glmopqrmp.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gdnoudcfe.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.hesvh.cn/Article/details/gfnynbqxv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/gdbyufttt.sHtML

[S40] C++：查找元素
来源：http://www.share.hesvh.cn/Article/details/gvvztivmh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gxlknjrph.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/genkowezo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gnjzlfjvh.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gryvptxna.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gzbtopazw.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gcqtivsvn.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fehbvm.com/Article/details/gldvzllpf.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gawdccekj.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/girtkoold.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gkxyckoyi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gjonxglxc.sHtML

[S46] C++：函数模板
来源：http://read.share.fehbvm.com/Article/details/gppfgzzdi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gajapzopj.sHtML


<!-- 参考信息 -->