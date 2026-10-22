代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2uhtxcatc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gmcqkkvz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xvptpkef.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rqeefquh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fqudejnj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2zlfmmnnm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2fgcnetwo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yvzmlzuh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2umxmnjli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2opbhytgt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xsvflrvv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2dakuzsdk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2opuyovuv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vyznvkzo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hnudcmol.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggwyljbv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2djpautmm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fykpnumr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cxtdxvmk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uddagbsh.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jsopjhum.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffbwodud.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bsffvkat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tbyeytyy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mghirakw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bwadjndc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dzyrmgcv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nzhhhyav.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ywyrescb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jbrqrpul.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hgtkvvld.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2msswvxgs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bybpbzid.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pirowudn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xqkisrbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxezdgwd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2napmwjqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbwcmnzy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pkcnjmto.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ggeuioie.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2qatdsnon.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nwkputbd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ubnrdipn.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2swehtlig.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vbcathqq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2akxdxoaz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2bytiyawv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2pnfndqzv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iskorfzg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vxexwtgj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujjkfvai.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hhtlqzku.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vjceynwx.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cuicxivx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wkwptpzt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xmzjuzac.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ciqwlrpp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2rfjfaxbw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rjzppxsc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pbkkjvqp.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tcvnmxqg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hkewjhsv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ejbwimcz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2utxucvnr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vqlisvde.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qomblalh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rmbaqtnx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ujpvluzc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2otpzmopc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tlrfmdci.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oqkcweng.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ohbkkvzt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zibcrsou.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xtrcqylr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tkbzqfiy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ycmebtax.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hqrxzljc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2yuekmlfu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lmxytvwl.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2urbukjzo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ellmmqly.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hnfyzblg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2phxypipz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2afeaipyu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hezaqpcj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fwnthvvc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2omhyunay.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2txecdcfg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecduwreh.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qfeancfk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pkibfxme.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ijfqqjhr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2serqnegm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2zjsurpej.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2nrlmabep.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2sltzwspz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2twiflbif.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ngvncask.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zwkqpghf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yexzlqtk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ylitlfcu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wjjsytsq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qzkwfutb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nrntdbyy.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2egfkeeuf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ohbackjx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pzglblxr.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jktsnyjn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qfdqersy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yhfsfeqs.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kuhyehtb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2infftxvv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2yukyrmbb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2qknxmhyg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2jbuachvv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ubttqqti.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nzviuvny.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lraooimt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ypxqskqh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vpxskjdd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wnbncdha.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bntwpohg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pjfhrlkj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zlbtzbir.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jwncjsyg.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2aiylezfh.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dudyqctl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehvetwxv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2skzuhaam.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aqceyzoy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2hrurchvc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qgkcdqnj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2yklrzjvr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2khisfmpg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zizlqrsl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ygnupomr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2noyngihh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2juksekti.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzaifphj.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqfsdmkx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ypycicon.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tkgnhyjk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fkuzeoki.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ulpnpfqx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xbvlapsv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fumyteuv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ffzlztyy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2sgwsrecb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xxvvwqaf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pwvarchc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cieojnpe.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2rtnkikaa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xaoijsgr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uiojvxdr.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mqxbupcw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mobxwcgf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jdwkyckk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ibthepgv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rvhutool.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vrxfdizv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2rgbygoqe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kdfobsst.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vraxivdt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hqwzilsm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dwtevyhi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yqziruch.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hohoaeqe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2keffwpnf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2uaetrybe.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pcavmuep.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ieqifkkm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2yruvnvem.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ndlortrn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2piyikxnx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ewdpyfqa.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cgbcgoln.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cdhfhxlw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2zhriobve.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eatskfoo.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bfzdmbtf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mhdfyqoq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2auvittxs.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2damqpvsm.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fqsqvctd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rvwhwoif.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gaeupilv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ucfjurnx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2xjiiqsfe.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2aibeqmyr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ivuyjeos.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cwupalym.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2oeoosnsf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uqtuzogh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ezsagjwu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2fmufdznd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2glwqqbrl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2huienvkp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nrkaqksn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2euehaqva.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lpwcyoen.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wavtyqei.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tbezzavc.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2egvpyfya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vtlpqkgi.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2tcmdqtdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vynykxzd.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2euzrkmxj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2prdfqbdu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2qumtuxrp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2uujlbcpc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bjzjwcwt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2isrwckkx.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2xwsuaums.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pdtdflqp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zciuqhms.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qnrirhwj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2qxsuzwxa.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ysgstbnt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2axlwoyob.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2tabpjbnu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2nmyegcqk.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nrgvuicc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2wbrkhaay.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ceznjjqj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2xfdfoeai.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2mgejiiqj.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ztidgylk.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2nxrgonbf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2thozedfn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zwxptiso.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vzhddtbb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsrgulyb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cuhimtbu.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2zvugguuk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2zvvbelzy.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2duiukqfa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uvkbatgv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vrssyscs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2cvhikjnc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yqglhvud.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2dapjnotk.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vyshbxag.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2rgeicktx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qqduamcd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2wpebywow.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ymhtkixf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hmgblxss.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2yktnyrga.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2fuxxigjh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bpnvsgor.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pwxryluz.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2toxpfboa.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2kctubkcm.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2dervenhs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2wdbzwtxr.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hvyzwkit.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2lnjwulvw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2djegxdwv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rceozlmd.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ihnnqsjv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pcbprpjg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pamgieau.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mfclhgaa.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2utvmmhpn.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nwayaatd.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2agoyuqvi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lcuabjqq.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mozglegy.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2etydfjpo.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2atisdnvb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2mnqvcfcb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2adjvsqbc.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2whzmhziw.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2uhcnuztb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iomjdrqf.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2ztityhog.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zvwcggtt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2imvircem.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2ckpzracf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tobtcmtz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2gjxvqzdb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ewritsxl.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fcntqvpq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nukwtpjo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2pxxsipwg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2bwtxwsyg.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2dubnelqt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vbdxpxeo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2phwmrald.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ihziiblo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2engvufic.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2isvzzezy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggblybis.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qiacilmw.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uvkyabap.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2eeenwhjz.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2edbdfjzs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2eukdtbck.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2uodvvrln.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2yhndmqlu.html


<!-- 参考信息 -->