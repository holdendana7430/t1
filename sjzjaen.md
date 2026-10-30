代发 wailian999

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyaoualm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmozlfven.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gltffhldk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvuyewvf.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjqmgfid.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/glpezagdx.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdxyjxdo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fanxiaobao.xyz/Article/details/gtegbxkwb.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gloymvegh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gexihryne.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gphgaebls.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuxxzofk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/ggjfuhbhi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glkfgpkah.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxqtczjo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhhakqxg.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdghavmq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcatojase.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gwerxdvgv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/grtzunkul.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikdbkvri.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmopmzudw.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gwgmldnuu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gzampghgq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzhadizv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gwdnacvbc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghlkmeqzg.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsifhswn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gallazmjc.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gngsimtav.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gekqowjei.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcintkads.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/getjoqvyt.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdsvcypog.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoayrest.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gjygbbdek.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/giocaxghl.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gdtvudmsh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzjdwrji.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gipyvkjso.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gmxlyvqeq.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcidaqtoa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gxvuaunjw.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gjdvrpink.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpatxucbq.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gwjygsatu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzuuwcwn.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzlqvbci.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gslkzkbzd.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlyyfils.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqbupzfrq.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ghvvijyin.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsjtyvutg.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeoakqmk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkggsyixk.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaxcazsu.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/ggxyxznor.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzatamdpk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghjhrcnjd.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstpisaau.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaohjqck.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsyfkalvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamfqvbbi.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxtqptsz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxiulgqmy.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeolqzrl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxxpahrs.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjodzegrr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaocrnwj.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzowvqkwf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmnffzpar.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gyjkhrynn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gesridvqr.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gvhncrdtm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlqrsxlw.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmouwixgo.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/geeeeooub.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghujezkal.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gabmktrkl.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjotitwbt.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givfhyydy.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/ggrwkusgb.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gldmxuvfd.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyimonoln.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fanxiaobao.xyz/Article/details/gjutqummw.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gyniwmrii.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaumnzbjb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzacdmuc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gulcurbia.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gnoxfuqui.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxxmhyyf.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gsabtimrt.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gpioddzmt.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gkxetofpo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gvanppmoy.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gbekweknw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxycqyfrl.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gqqnekngb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbtnqxa.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gcdfcvbcb.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grnkpnrtt.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gminznlkl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gacthywmw.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxkqnzo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmtipxgj.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gpunlbfzf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gikhkxhsi.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gvsiaityt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gbcqmdqlp.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gukkgenlv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/ghhkkmzpt.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuuojxvd.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjegnjdsg.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzvraeie.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gwmumbxuz.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfzczlbd.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gpugtsksg.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gskteqjpy.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gknwduffo.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxozhxrx.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiplxqzo.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwhgjtfj.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyffllpdi.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxnhrhgox.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelfgttzn.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/glnopqqti.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/grgtvfhkx.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gmavvclzm.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqrdtqor.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gzuyvdlat.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gycavsqmp.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcuytxrk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gstbjqwgq.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gqcfcfaqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gfojvhvom.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaeztagx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazgfylwx.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnswidokk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnrndujpl.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/ghunqqrwd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gmlvlmnkj.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuexoeer.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gglvvcwtd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgidxlul.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbfzauols.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdruukyn.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guouxwbhg.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbpxmcxy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gomkhelnv.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwwhxbea.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwhtrpgu.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gzsqqifqb.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwwwvkmp.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gixrukhea.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gzztgimqt.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gzrjeggpj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gdykmntdq.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gmvhnrefe.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gwmpvtynl.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gignzbyto.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gzkijrkof.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gobcjhipz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyxdtrit.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgvlyzjw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gbradwzdy.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gjetdoeje.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsjuhper.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxfbmyjl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/glxungajz.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnvqnmrv.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkmzffye.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gdqngazbv.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzgfehtm.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gskklvooa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpjephjxo.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/galavmogb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gampoitlv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdztisgcs.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnibwktk.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gsgovyufm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/guxyacuqi.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gujefnhvy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlrmzvs.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/guynzqjpb.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gfkvqkeay.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxwejeve.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvttetiua.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvoqueljs.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gebyykigh.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfcqbvor.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gchyzcvld.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/greqlqjyc.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsybvfhm.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnumwfwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gequpizzy.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbascznq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gprfidmod.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxnkoydo.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gkxqgmzoc.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gadexwjmm.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/goncrzhsb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gauvndlxh.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvcahuto.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gjvuqjdcr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvrewuyha.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzspkyai.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqwtglgb.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpswfrrkp.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/glvzjkuke.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/glhglxuab.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjxhmlwr.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gczoperld.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyrnihzc.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbpqqoqc.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpfnrjzv.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbebpyxl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnsbosk.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gfqtlnqsn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgsbespk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxncvldy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtzbckcj.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gdomicfgu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgaxfaov.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkowpfmgs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsagchvkf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ggbmpiaih.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/giugwdzee.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctidvpiw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtztxofpk.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gtlvqsrvp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsdirfod.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkuwsatc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gpxzadqkn.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqhxtmlf.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gghvmqndc.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gomnypfkl.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtbloibz.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gstczmirm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genodxefn.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcmihtaf.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gsmwssqwp.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gbgoayxtv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcnefjvz.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/glbcmaogv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gieniywvb.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gswkpmzdx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxkjwpll.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtkdmvjs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gbtbyvvpt.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/guzmhjcof.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gukphrbyo.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyynshyd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvmgbioa.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmfdnpqj.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gusceisda.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdtftvp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/glovjnkcp.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaehoiyy.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmdkwdevv.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdymcqfb.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gstuvtghv.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktxtvzbv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gebsnidfo.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/glgxzwwec.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gzmydxfvm.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnlxrcej.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/grdrirgip.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gtudkisxg.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gzoaoulsm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgpbqomq.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gwptmposd.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpsenwblh.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gitondxnf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gbsjdmeav.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/gcwuvjtei.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhnigwgy.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmubvgou.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gpoaeqrfu.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gpujbhcln.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpevktjx.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gevqdegci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtleqylml.sHtML

[S38] C++：排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gajvemxxd.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/goscaolfw.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqddqohn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gwhmgtczo.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gskrkbfhz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gstwqziti.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbovjvzmo.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/geyfigymn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmlmsptd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxjbcsnk.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/ghophfdda.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gtbtrusvb.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grrcfctbv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvczvjwiq.sHtML

[S45] C++：lambda
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnnvvyjn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlpxmfgi.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmrnkbyw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicdnxfem.sHtML


<!-- 参考信息 -->